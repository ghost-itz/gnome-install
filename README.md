# gnome-install

iwcttl
device list
station "dispositivo" scan
station "dispositivo" get-networks
station "dispositivo" connect SSID

  cfdisk
  mkfs.ext4 /dev/sda...
  mkswap /dev/sda...
  swapon /dev/sda...

  mount /dev/sda... /mnt

pacstrap -i /mnt base base-devel linux-lts linux-firmnware nano linux-lts-headers git

genfstab -U -p /mnt >> /mnt/etc/fstab
arch-chroot /mnt

mkdir /boot/efi
mount /dev/sda1 /boot/efi

nano /etc/locale.gen
  locale-gen

