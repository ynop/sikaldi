Bootstrap: docker
Registry: nvcr.io
From: nvidia/pytorch:19.09-py3

%runscript

    echo "Nothing to do here."

%post

    apt-get update
    apt-get install -y libsndfile1
    apt-get install -y sox
    apt-get install -y python3-pip
    rm -rf /var/lib/apt/lists/*

    pip3 install --disable-pip-version-check -U pandas==0.24.2 tqdm==4.31.1 ascii-graph==1.5.1 wrapt==1.10.11 librosa toml soundfile ipdb
