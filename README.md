# Basics of NixOS

## Table of Contents

<details open>

<summary>ToC Drop Down</summary>

1. [About](#about)
2. [Initial Install](#initial-install)
3. [NixOS Config](#nixos-config)
4. [bpswm Config](#bpswm-config)
5. [sxhkd Config](#sxhkd-config)

</details>


## About
This repository is to document the set up of a single-boot fresh install of NixOS and configuration that suits my needs.

NixOS is different from the usual OS in that you edit and maintain a config file in which you declare the packages you want included. 

## Initial Install

<details>
<summary>A. Getting the Media</summary>

1. Download a NixOS image from https://nixos.org/download


> ⚠️ Please note that Nix is a package manager and NixOS is an operating system (that uses Nix) and both are available through this page. Be wary of following the incorrect installation procedure. 

I will be using the Plasma Desktop 64-bit Intel/AMD version initially. Be sure to grab what matches your architecture and desires. 

2. Mount `nixos.iso` to a USB drive. 

I use Balena Etcher in most cases https://etcher.balena.io/ . It's incredibly stream-lined and I have yet to have an issue due to it.

3. Insert the USB drive into a USB port on the machine you would like to modify.

4. Restart or power up the machine.

</details>

<details>
<summary>B. Booting From USB</summary>

1. Boot from your USB drive

If your system is not already setup to boot from USB you will need to press the BIOS key while your machine is booting. 

> Most common BIOS keys are `DEL` or `F2` but that's not always the case. My current BIOS key is `F12`. You can check your motherboard's instruction manual to see which key is designated as your BIOS key. Some machines show which is your BIOS key on startup. 

2. Change USB to be first in boot order

3. Restart the machine

</details>