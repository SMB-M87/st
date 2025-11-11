# st
Suckless simple terminal
git clone https://git.suckless.org/st
cd /st

## Patches
curl -O https://st.suckless.org/patches/alpha/st-alpha-20240814-a0274bc.diff

curl -O https://st.suckless.org/patches/gruber-darker/st-gruber-darker-0.9.2.diff

curl -O https://st.suckless.org/patches/clipboard/st-clipboard-0.8.3.diff

curl -O https://st.suckless.org/patches/scrollback/st-scrollback-0.9.2.diff

curl -O https://st.suckless.org/patches/scrollback/st-scrollback-reflow-0.9.2.diff

curl -O https://st.suckless.org/patches/scrollback/st-scrollback-mouse-0.9.2.diff

curl -O  https://st.suckless.org/patches/scrollback/st-scrollback-mouse-altscreen-20220127-2c5edf2.diff

## Apply Patches & Build
patch -p1 < st-alpha-20240814-a0274bc.diff

patch -p1 < st-gruber-darker-0.9.2.diff

patch -p1 < st-clipboard-0.8.3.diff

patch -p1 < st-scrollback-0.9.2.diff

patch -p1 < st-scrollback-reflow-0.9.2.diff

patch -p1 < st-scrollback-mouse-0.9.2.diff

patch -p1 < st-scrollback-mouse-altscreen-20220127-2c5edf2.diff

nvim config.def.h

        font > size

make clean install
