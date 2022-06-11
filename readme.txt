# Environment
Ubuntu 18.04.6 LTS
python requirements(mostly required)
# Name                    Version                   Build  Channel
imagecodecs               2021.11.20               pypi_0    pypi
imageio                   2.19.2                   pypi_0    pypi
intel-openmp              2021.4.0          h06a4308_3561
ipython                   7.32.0                   pypi_0    pypi
jpeg                      9d                   h7f8727e_0
matplotlib                3.5.1            py37h06a4308_1
matplotlib-base           3.5.1            py37ha18d171_1
matplotlib-inline         0.1.3                    pypi_0    pypi
numpy                     1.21.2           py37h20f2e39_0
numpy-base                1.21.2           py37h79a1101_0
opencv-python             4.5.5.64                 pypi_0    pypi
openh264                  2.1.1                h4ff587b_0
openssl                   1.1.1n               h7f8727e_0
packaging                 21.3               pyhd3eb1b0_0
pandas                    1.3.5                    pypi_0    pypi
pillow                    9.0.1            py37h22f2fdc_0
python                    3.7.3                h0371630_0
python-dateutil           2.8.2              pyhd3eb1b0_0
pytorch                   1.11.0          py3.7_cuda10.2_cudnn7.6.5_0    pytorch
pytorch-mutex             1.0                        cuda    pytorch
pytz                      2022.1                   pypi_0    pypi
scikit-image              0.19.2                   pypi_0    pypi
scikit-learn              1.0.2                    pypi_0    pypi
scipy                     1.7.3                    pypi_0    pypi
torchaudio                0.11.0               py37_cu102    pytorch
torchvision               0.12.0               py37_cu102    pytorch
tornado                   6.1              py37h27cfd23_0
tqdm                      4.64.0                   pypi_0    pypi

# Train and test the model

Test the pretrained model, results will be stored in ../experiment/test_drive_k8_10_epoch_pc and ../experiment/test_chase_k8_10_epoch_pc
	cd model_training
	bash run_test.sh
notion： take care of the args： -n_GPUs 1 --id_GPU 0，n_GPUs is the number of GPUs you want to use and id_GPU is the id of the first GPU used.

Train the model, results will be stored in ../experiment/drive_k8_10_epoch_pc and ../experiment/chase_k8_10_epoch_pc
	cd model_training
	bash run_train.sh
	bash run_train_chase.sh
notion： take care of the args： -n_GPUs 1 --id_GPU 0，n_GPUs is the number of GPUs you want to use and id_GPU is the id of the first GPU used.

# results
drive_k8_10_epoch_pc
Acc: 0.9707834  |  Se: 0.8295803 |  Sp: 0.98454344 |  Auc: 0.9883818553310141 |  Background_IOU: 0.9684946 |  vessel_IOU: 0.7122363 
[DRIVET x1]     DICE Score: 0.831767 (Best: 0.831767 @epoch 9)

chase_k8_10_epoch_pc
Acc: 0.97660536  |  Se: 0.8686458 |  Sp: 0.98388076 |  Auc: 0.9920686277064172 |  Background_IOU: 0.97522855 |  vessel_IOU: 0.7011959 
[CHASET x1]     DICE Score: 0.824195 (Best: 0.824195 @epoch 9)






# python environment(all packets)
# Name                    Version                   Build  Channel
_libgcc_mutex             0.1                        main
_openmp_mutex             4.5                       1_gnu
backcall                  0.2.0                    pypi_0    pypi
blas                      1.0                         mkl
brotli                    1.0.9                he6710b0_2
brotlipy                  0.7.0           py37h27cfd23_1003
bzip2                     1.0.8                h7b6447c_0
ca-certificates           2022.3.18            h06a4308_0
certifi                   2021.10.8        py37h06a4308_2
cffi                      1.15.0           py37h7f8727e_0
charset-normalizer        2.0.4              pyhd3eb1b0_0
cryptography              36.0.0           py37h9ce1e76_0
cudatoolkit               10.2.89              hfd86e86_1
cycler                    0.11.0             pyhd3eb1b0_0
dbus                      1.13.18              hb2f20db_0
decorator                 5.1.1                    pypi_0    pypi
expat                     2.4.4                h295c915_0
ffmpeg                    4.3                  hf484d3e_0    pytorch
fontconfig                2.13.1               h6c09931_0
fonttools                 4.25.0             pyhd3eb1b0_0
freetype                  2.11.0               h70c0345_0
giflib                    5.2.1                h7b6447c_0
glib                      2.63.1               h5a9c865_0
gmp                       6.2.1                h2531618_2
gnutls                    3.6.15               he1e5248_0
gst-plugins-base          1.14.0               hbbd80ab_1
gstreamer                 1.14.0               hb453b48_1
icu                       58.2                 he6710b0_3
idna                      3.3                pyhd3eb1b0_0
imagecodecs               2021.11.20               pypi_0    pypi
imageio                   2.19.2                   pypi_0    pypi
intel-openmp              2021.4.0          h06a4308_3561
ipython                   7.32.0                   pypi_0    pypi
jedi                      0.18.1                   pypi_0    pypi
joblib                    1.1.0                    pypi_0    pypi
jpeg                      9d                   h7f8727e_0
kiwisolver                1.3.2            py37h295c915_0
lame                      3.100                h7b6447c_0
lcms2                     2.12                 h3be6417_0
libedit                   3.1.20210910         h7f8727e_0
libffi                    3.2.1             hf484d3e_1007
libgcc-ng                 9.3.0               h5101ec6_17
libgomp                   9.3.0               h5101ec6_17
libiconv                  1.15                 h63c8f33_5
libidn2                   2.3.2                h7f8727e_0
libpng                    1.6.37               hbc83047_0
libstdcxx-ng              9.3.0               hd4cf53a_17
libtasn1                  4.16.0               h27cfd23_0
libtiff                   4.2.0                h85742a9_0
libunistring              0.9.10               h27cfd23_0
libuuid                   1.0.3                h7f8727e_2
libuv                     1.40.0               h7b6447c_0
libwebp                   1.2.2                h55f646e_0
libwebp-base              1.2.2                h7f8727e_0
libxcb                    1.14                 h7b6447c_0
libxml2                   2.9.12               h03d6c58_0
lz4-c                     1.9.3                h295c915_1
matplotlib                3.5.1            py37h06a4308_1
matplotlib-base           3.5.1            py37ha18d171_1
matplotlib-inline         0.1.3                    pypi_0    pypi
mkl                       2021.4.0           h06a4308_640
mkl-service               2.4.0            py37h7f8727e_0
mkl_fft                   1.3.1            py37hd3c417c_0
mkl_random                1.2.2            py37h51133e4_0
munkres                   1.1.4                      py_0
ncurses                   6.3                  h7f8727e_2
nettle                    3.7.3                hbbd107a_1
networkx                  2.6.3                    pypi_0    pypi
numpy                     1.21.2           py37h20f2e39_0
numpy-base                1.21.2           py37h79a1101_0
opencv-python             4.5.5.64                 pypi_0    pypi
openh264                  2.1.1                h4ff587b_0
openssl                   1.1.1n               h7f8727e_0
packaging                 21.3               pyhd3eb1b0_0
pandas                    1.3.5                    pypi_0    pypi
parso                     0.8.3                    pypi_0    pypi
pcre                      8.45                 h295c915_0
pexpect                   4.8.0                    pypi_0    pypi
pickleshare               0.7.5                    pypi_0    pypi
pillow                    9.0.1            py37h22f2fdc_0
pip                       21.2.2           py37h06a4308_0
prompt-toolkit            3.0.28                   pypi_0    pypi
ptyprocess                0.7.0                    pypi_0    pypi
pycparser                 2.21               pyhd3eb1b0_0
pygments                  2.11.2                   pypi_0    pypi
pyopenssl                 22.0.0             pyhd3eb1b0_0
pyparsing                 3.0.4              pyhd3eb1b0_0
pyqt                      5.9.2            py37h05f1152_2
pysocks                   1.7.1                    py37_1
python                    3.7.3                h0371630_0
python-dateutil           2.8.2              pyhd3eb1b0_0
pytorch                   1.11.0          py3.7_cuda10.2_cudnn7.6.5_0    pytorch
pytorch-mutex             1.0                        cuda    pytorch
pytz                      2022.1                   pypi_0    pypi
pywavelets                1.3.0                    pypi_0    pypi
qt                        5.9.7                h5867ecd_1
readline                  7.0                  h7b6447c_5
requests                  2.27.1             pyhd3eb1b0_0
scikit-image              0.19.2                   pypi_0    pypi
scikit-learn              1.0.2                    pypi_0    pypi
scipy                     1.7.3                    pypi_0    pypi
setuptools                58.0.4           py37h06a4308_0
sip                       4.19.8           py37hf484d3e_0
six                       1.16.0             pyhd3eb1b0_1
sqlite                    3.33.0               h62c20be_0
threadpoolctl             3.1.0                    pypi_0    pypi
tifffile                  2021.11.2                pypi_0    pypi
tk                        8.6.11               h1ccaba5_0
torchaudio                0.11.0               py37_cu102    pytorch
torchvision               0.12.0               py37_cu102    pytorch
tornado                   6.1              py37h27cfd23_0
tqdm                      4.64.0                   pypi_0    pypi
traitlets                 5.1.1                    pypi_0    pypi
typing_extensions         4.1.1              pyh06a4308_0
urllib3                   1.26.8             pyhd3eb1b0_0
wcwidth                   0.2.5                    pypi_0    pypi
wheel                     0.37.1             pyhd3eb1b0_0
xz                        5.2.5                h7b6447c_0
zlib                      1.2.11               h7f8727e_4
zstd                      1.4.9                haebb681_0