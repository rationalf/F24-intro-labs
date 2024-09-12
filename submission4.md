# Lab-4

1) Create repository and download to it opera-stable.deb
2) Compress it to package arhive
3)Add this repository to my source list (with one error N: Download is performed unsandboxed as root as file '/home/sergey/local-apt-repo/./InRelease' couldn't be accessed by user '_apt'. - pkgAcquire::Run (13: Permission denied))
4) verify it without problem
5)install packages

## Task 2

1)opera-stable:
  Installed: (none)
  Candidate: 113.0.5230.86
  Version table:
     113.0.5230.86 500
        500 file:/home/sergey/local-apt-repo ./ Packages
2)Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  adwaita-icon-theme alsa-topology-conf alsa-ucm-conf at-spi2-core chromium-codecs-ffmpeg-extra
  dconf-gsettings-backend dconf-service fontconfig gsettings-desktop-schemas gtk-update-icon-cache hicolor-icon-theme
  humanity-icon-theme libasound2 libasound2-data libatk-bridge2.0-0 libatk1.0-0 libatk1.0-data libatspi2.0-0
  libavahi-client3 libavahi-common-data libavahi-common3 libcairo-gobject2 libcairo2 libcolord2 libcups2 libdatrie1
  libdconf1 libdouble-conversion3 libdrm-amdgpu1 libdrm-intel1 libdrm-nouveau2 libdrm-radeon1 libegl-mesa0 libegl1
  libepoxy0 libevdev2 libgbm1 libgdk-pixbuf-2.0-0 libgdk-pixbuf2.0-bin libgdk-pixbuf2.0-common libgl1 libgl1-amber-dri
  libgl1-mesa-dri libglapi-mesa libglvnd0 libglx-mesa0 libglx0 libgraphite2-3 libgtk-3-0 libgtk-3-bin libgtk-3-common
  libgudev-1.0-0 libharfbuzz0b libice6 libinput-bin libinput10 liblcms2-2 libllvm15 libmd4c0 libmtdev1 libnspr4
  libnss3 libpango-1.0-0 libpangocairo-1.0-0 libpangoft2-1.0-0 libpciaccess0 libpcre2-16-0 libpixman-1-0 libqt5core5a
  libqt5dbus5 libqt5gui5 libqt5network5 libqt5svg5 libqt5widgets5 librsvg2-2 librsvg2-common libsensors-config
  libsensors5 libsm6 libthai-data libthai0 libwacom-bin libwacom-common libwacom9 libwayland-client0
  libwayland-cursor0 libwayland-egl1 libwayland-server0 libx11-xcb1 libxcb-dri2-0 libxcb-dri3-0 libxcb-glx0
  libxcb-icccm4 libxcb-image0 libxcb-keysyms1 libxcb-present0 libxcb-randr0 libxcb-render-util0 libxcb-render0
  libxcb-shape0 libxcb-shm0 libxcb-sync1 libxcb-util1 libxcb-xfixes0 libxcb-xinerama0 libxcb-xinput0 libxcb-xkb1
  libxcomposite1 libxcursor1 libxdamage1 libxfixes3 libxi6 libxinerama1 libxkbcommon-x11-0 libxkbcommon0 libxrandr2
  libxrender1 libxshmfence1 libxtst6 libxxf86vm1 qt5-gtk-platformtheme qttranslations5-l10n session-migration
  ubuntu-mono x11-common
Suggested packages:
  libasound2-plugins alsa-utils colord cups-common gvfs liblcms2-utils qt5-image-formats-plugins qtwayland5
  librsvg2-bin lm-sensors
The following NEW packages will be installed:
  adwaita-icon-theme alsa-topology-conf alsa-ucm-conf at-spi2-core chromium-codecs-ffmpeg-extra
  dconf-gsettings-backend dconf-service fontconfig gsettings-desktop-schemas gtk-update-icon-cache hicolor-icon-theme
  humanity-icon-theme libasound2 libasound2-data libatk-bridge2.0-0 libatk1.0-0 libatk1.0-data libatspi2.0-0
  libavahi-client3 libavahi-common-data libavahi-common3 libcairo-gobject2 libcairo2 libcolord2 libcups2 libdatrie1
  libdconf1 libdouble-conversion3 libdrm-amdgpu1 libdrm-intel1 libdrm-nouveau2 libdrm-radeon1 libegl-mesa0 libegl1
  libepoxy0 libevdev2 libgbm1 libgdk-pixbuf-2.0-0 libgdk-pixbuf2.0-bin libgdk-pixbuf2.0-common libgl1 libgl1-amber-dri
  libgl1-mesa-dri libglapi-mesa libglvnd0 libglx-mesa0 libglx0 libgraphite2-3 libgtk-3-0 libgtk-3-bin libgtk-3-common
  libgudev-1.0-0 libharfbuzz0b libice6 libinput-bin libinput10 liblcms2-2 libllvm15 libmd4c0 libmtdev1 libnspr4
  libnss3 libpango-1.0-0 libpangocairo-1.0-0 libpangoft2-1.0-0 libpciaccess0 libpcre2-16-0 libpixman-1-0 libqt5core5a
  libqt5dbus5 libqt5gui5 libqt5network5 libqt5svg5 libqt5widgets5 librsvg2-2 librsvg2-common libsensors-config
  libsensors5 libsm6 libthai-data libthai0 libwacom-bin libwacom-common libwacom9 libwayland-client0
  libwayland-cursor0 libwayland-egl1 libwayland-server0 libx11-xcb1 libxcb-dri2-0 libxcb-dri3-0 libxcb-glx0
  libxcb-icccm4 libxcb-image0 libxcb-keysyms1 libxcb-present0 libxcb-randr0 libxcb-render-util0 libxcb-render0
  libxcb-shape0 libxcb-shm0 libxcb-sync1 libxcb-util1 libxcb-xfixes0 libxcb-xinerama0 libxcb-xinput0 libxcb-xkb1
  libxcomposite1 libxcursor1 libxdamage1 libxfixes3 libxi6 libxinerama1 libxkbcommon-x11-0 libxkbcommon0 libxrandr2
  libxrender1 libxshmfence1 libxtst6 libxxf86vm1 opera-stable qt5-gtk-platformtheme qttranslations5-l10n
  session-migration ubuntu-mono x11-common

## Task 3

1) sudo apt-mark hold opera-stable

2) apt-mark showhold (output:opera-stable) (list op packages)

3) sudo apt-mark unhold opera-stable (output:Canceled hold on opera-stable.)