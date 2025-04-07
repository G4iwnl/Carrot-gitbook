# 시뮬레이터

## [vmware work statation 설치](https://support.broadcom.com/group/ecx/productdownloads?subfamily=VMware+Workstation+Pro)

* 개인사용은 공짜
* 다운받아서 설치함

## [ubuntu 24.04설치](https://releases.ubuntu.com/noble/ubuntu-24.04.1-desktop-amd64.iso)

* 3d accelerator disable하고설치함

## VMware Tools설치

* sudo apt update
* sudo apt install open-vm-tools-desktop

## 그래픽드라이버설치

* sudo add-apt-repository ppa:oibaf/graphics-drivers
* sudo apt update
* sudo apt upgrade

## vmware 설정변경

* 3d accelerator enable

## comma openpilot설치

* git clone -b master --recurse-submodules [https://github.com/commaai/openpilot](https://github.com/commaai/openpilot) comma
* cd comma
* git lfs pull

## carrot openpilot 설치

* git clone -b v7-wip3-wd40 [https://github.com/ajouatom/openpilot](https://github.com/ajouatom/openpilot) carrot

## 환경설정 및 빌드

* cd comma/tools
* ./ubuntu\_setup.sh
* cd ..
* source .venv/bin/activate
* scons -u -j$(nproc)

## 시뮬레이터 실행해보기

* t**erminal 창두개 열기**
* sudo apt install pocl-opencl-icd
* cd comma
* source .venv/bin/active
* tools/sim/run\_bridge.py (1번창)
* tools/sim/launch\_openpilot.sh (2번창)
* 1번창에서 (1,2,3, w, a, d, z, x) 키로 조작함.
