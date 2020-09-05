# manifest-kmtek-stm32mp

- `mkdir yocto-kmtek`
- `cd yocto-kmtek`
- `repo init -u https://github.com/thanhduongvs/manifest-kmtek-stm32mp.git -b dunfell`
- `repo sync -j8`
- `DISTRO=openstlinux-weston MACHINE=kmtek source layers/meta-st/scripts/envsetup.sh build`
- `bitbake kmtek-weston --runall=fetch`
- `bitbake -k kmtek-weston`