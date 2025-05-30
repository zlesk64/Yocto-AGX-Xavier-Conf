# Yocto-AGX-Xavier-Conf
Repository to keep and track configuration files for building yocto linux for the Nvidia Jetson AGX Xavier.

The two conf files go in `<yocto_working_dir>/build/conf/` 

Currently if being built on an ubuntu 24.04 or higher host bitbake will fail to start compiling yocto because of apparmor denying bitbake to create user namespaces. You can temporarily bypass this by running the following as root: `apparmor_parser -R /etc/apparmor.d/unprivileged_userns` 



