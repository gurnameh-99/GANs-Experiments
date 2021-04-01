Method to install magenta in ubuntu 20.04:
[2:37 PM]
- git clone https://github.com/tensorflow/magenta.git
- do pip install -e . inside magenta repo
- do  sudo apt-get install libjack-dev and sudo apt-get install libasound2-dev to install alsa and jack
GitHub
magenta/magenta
Magenta: Music and Art Generation with Machine Intelligence - magenta/magenta

[2:38 PM]
Download these 2:
-  https://storage.googleapis.com/magentadata/models/gansynth/acoustic_only.zip
- https://storage.googleapis.com/magentadata/models/gansynth/all_instruments.zip
[2:38 PM]
and put it inside the magenta repo or wherever u like
[2:39 PM]
Then it's ready to generate some sounds:
- python magenta/models/gansynth/gansynth_generate.py --ckpt_dir=/path/to/acoustic_only --output_dir=/path/to/output/dir --midi_file=/path/to/file.mid
- gansynth_generate --ckpt_dir=/path/to/acoustic_only --output_dir=/path/to/output/dir --midi_file=/path/to/file.mid
Use above commands to run pretrained models
