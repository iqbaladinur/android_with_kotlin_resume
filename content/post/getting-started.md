---
title: Getting Started
description: Memulai belajar android development dg kotlin.
author: Iqbal Adi Nurmansyah
publishedAt: 2020-08-10T10:07:33.402Z
category: android
---


### Pembukaan

Sebelumnya di tahun 2016 atau 2017 saya pernah mempelajari android development dengan java, waktu itu sudah cukup familiar dengan IDE android studio. Jadi tutorial perjalanan ini mungkin tidak akan sedetail mungkin atau benar-benar dari 0, namun akan saya mulai dari penginstalan IDE.

Spek pc/laptop yang saya gunakan:
- OS: ubuntu 20.04
- processor: core i3 6006U
- ram: 2x 4gb
- memory: ssd 128gb nvme + ssd 256gb
- vga: nvidia gt750 or something, saya lupa

Rekomendasi spek <b> diatas i3, pakai ssd, ram > 8 gb </b>

### Install android studio

Karena saya peralihan ke linux, jadi saya memilih install android studio dari snapstore <a href="https://snapcraft.io/android-studio">Link android studio</a>. Process installasi sama dengan pada umumnya, kalau di awal akan di suruh memilih lokasi sdk. Kalian taruh di drive yang agak longgar. Pengalaman saya next2 aja, tapi lupa direktori `/home` saya pas install ubuntu cuma tak kasih 15gb, alhasil harus mindahin ke partisi lainnya kemarin. Tunggu process installasi selesai. Tentu usahakan internet connected, karena android studionya akan download beberapa package yang dia butuhkan.

<div align="center">
  <img src="https://raw.githubusercontent.com/iqbaladinur/android_with_kotlin_resume/master/resource/as.png" alt="android studio">
  <p class="text-center text-xs">
    Android Studio
  </p>
</div>

Setelah muncul Gambar seperti diatas, pilih configure dan pilih menu sdk manager. Download sdk atau versi android yang akan dibuat aplikasinya.

Setupt `PATH` atau environtment variable. Referensi <a href="https://developer.android.com/studio/command-line/variables"> link </a>, setup env ini kalau ingin mengubah lokasi-lokasi dari component android studio. Misalnya ingin memindahkan lokasi `avd` atau emulator, sdk dll. Dalam kasus saya, saya butuh supaya beberapa tool tersebut bisa jalan lewat command line atau terminal. Berikut setup path yang saya pakai untuk config bash saya:

```bash
export ANDROID_SDK_ROOT=/path/to/your/Android/Sdk
export PATH=$PATH:$ANDROID_SDK_ROOT/emulator
export PATH=$PATH:$ANDROID_SDK_ROOT/tools
export PATH=$PATH:$ANDROID_SDK_ROOT/tools/bin
export PATH=$PATH:$ANDROID_SDK_ROOT/platform-tools
```

kalau di windows edit path environtment variable. Jika sudah tes dengan run `adb` atau `emulator`.

### Membuat Proyek

Turorial yang saya ikuti adalah kurikulum google, [link](https://codelabs.developers.google.com/android-kotlin-fundamentals/).
- Pertama buka android studio
- pilih `start a new android studio project`
- pilih template `empty activity` 
- isi data applikasi terserah
- pilih `language kotlin`
- tentukan minimum sdk(android version)

### Fundamental Android

Beberapa fundamental android yang saya tangkap hari ini.

**Activity**

Dalam activity ada beberapa lifecycle activity, yang baru saya pelajari adalah `oncreate` di dalam `oncreate` ini kita membinding view dan component yang akan di gunakan dalam sebuah activity.

**Resource**

Di dalam resource ini digunakan untuk menyimpan view, layout, component, atau static asset lainnya.

Bersambung.

Nb. Codelab ikuti saja di link google, artikel ini hanya untuk merecord pembelajaran saya.