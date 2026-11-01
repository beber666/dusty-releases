# Dusty — Linux packages

**Dusty** prepares and runs the machining of your parts on a CNC router: design, toolpaths (profile, pocket, V-carving,
drilling…), a 3D preview of the machined part, G-code in 14 flavors, and control of GRBL, grblHAL, FluidNC, Duet, Marlin and
Smoothieware machines over USB or the network. A built-in virtual CNC lets you try everything without a machine. Free, with
no account, no subscription and no ads.
Website: <https://dusty.websolutis.com/>

This repository only hosts the **Linux packages** of Dusty (its source code is not public):

- **Releases**: `.deb` packages (x86_64 and ARM 64-bit, e.g. Raspberry Pi), AppImage and Flatpak bundles.
- **APT repository**: install and updates through `apt` on Debian, Ubuntu, Linux Mint and Raspberry Pi OS:

  ```sh
  curl -fsSL https://beber666.github.io/dusty-releases/dusty.gpg | sudo tee /usr/share/keyrings/dusty.gpg > /dev/null
  echo "deb [signed-by=/usr/share/keyrings/dusty.gpg] https://beber666.github.io/dusty-releases stable main" | sudo tee /etc/apt/sources.list.d/dusty.list
  sudo apt update && sudo apt install dusty
  ```

- **Flatpak repository**: install and updates on any distribution with Flatpak (x86_64 and ARM 64-bit):

  ```sh
  flatpak install --user https://beber666.github.io/dusty-releases/flatpak/dusty.flatpakref
  ```

- **Snap Store** and **AUR** (coming soon).

USB machines: your account must be a member of the `dialout` group
(`sudo usermod -aG dialout $USER`, then log out and back in).

---

**Dusty** prépare et pilote l'usinage de vos pièces sur une fraiseuse CNC. Ce dépôt n'héberge que les **paquets Linux** de
Dusty (le code n'est pas public) : paquets `.deb` (x86_64 et ARM 64 bits, Raspberry Pi), AppImage et Flatpak dans les
« Releases », dépôt APT et dépôt Flatpak (commandes ci-dessus, mises à jour comprises), bientôt le Snap Store et l'AUR.
Site : <https://dusty.websolutis.com/fr/>

© 2026 Websolutis. Dusty is free to download and use; redistribution of these packages is allowed unchanged.
