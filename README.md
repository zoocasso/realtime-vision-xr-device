<div align="center">

# 🥽 Real-Time Vision Enhancement for XR Headset

**2024 Pangyo XR Device Makerthon — Team Lead (5-person laboratory team)**

[![EN](https://img.shields.io/badge/Language-English-blue?style=flat-square)](#-english)
[![KR](https://img.shields.io/badge/언어-한국어-red?style=flat-square)](#-한국어)

</div>

---

## 🇺🇸 English

A wearable real-time vision enhancement system for the **Metalens 2 XR headset**, designed to restore visibility in fog and low-light conditions through optical-imaging algorithms deployed on embedded ARM64 hardware.

### 📋 Project Overview

An end-to-end XR vision enhancement pipeline that addresses two critical failure modes of outdoor wearable displays: atmospheric scattering (fog) and photon starvation (low-light). The system targets disaster response, nighttime driving, and industrial inspection scenarios where visual impairment directly affects user safety.

- **Event:** 2024 Pangyo XR Device Makerthon
- **Role:** Team lead of a five-person laboratory team — concept, task allocation, core algorithm implementation, C++/Unity integration, on-stage presentation
- **Target Device:** Metalens 2 XR Headset (ARM64)
- **This repository:** presentation slides (`PPT-XR-DEVICE.pdf`) and project summary; the source code is not published.

### ✨ Key Contributions

- **Fourier Peplography for Dehazing** — Implemented a physics-based image recovery algorithm that leverages spatial-frequency synthesis to remove scattering artifacts caused by atmospheric haze.
- **Photon Counting for Low-Light Recovery** — Built a photon-counting pipeline that recovers usable images from low-light sensor input.
- **On-Device Deployment** — Wrote the core in C++/OpenCV and built it as an Android native plugin (`.so`, arm64) loaded by a Unity (IL2CPP) app on the headset, using only the device camera.

### 🛠 Tech Stack

| Layer | Technology |
|---|---|
| **Algorithms** | Fourier Peplography, Photon Counting |
| **Core** | C++, OpenCV (Android native build, arm64) |
| **Integration** | Unity (IL2CPP) ↔ Android native plugin (`.so`) |
| **Hardware** | Metalens 2 XR Headset |

### 🎯 Outcome

Delivered a working prototype at the Makerthon showcase, demonstrating live dehazing and low-light enhancement through the XR headset. Presented the optical-imaging principles and real-time implementation strategy to judges and industry attendees.

<div align="right"><a href="#-한국어">🇰🇷 한국어로 보기 ↓</a></div>

---

## 🇰🇷 한국어

**Metalens 2 XR 헤드셋**을 위한 실시간 시각 개선 시스템으로, 광학 이미징 알고리즘을 ARM64 임베디드 하드웨어에 탑재하여 안개 및 저조도 환경에서의 가시성을 복원합니다.

### 📋 프로젝트 개요

야외용 웨어러블 디스플레이의 두 가지 치명적 한계 — 대기 산란(안개)과 광자 부족(저조도) — 을 해결하는 end-to-end XR 시각 개선 파이프라인입니다. 시각 손상이 사용자 안전에 직결되는 재난 대응, 야간 주행, 산업 검사 환경을 타겟으로 합니다.

- **행사:** 2024 판교 XR Device 메이커톤
- **역할:** 연구실 5인 팀 리드 — 기획, 역할 분담, 핵심 알고리즘 구현, C++/Unity 연동, 현장 발표
- **타겟 하드웨어:** Metalens 2 XR Headset (ARM64)
- **이 저장소:** 발표자료(`PPT-XR-DEVICE.pdf`)와 프로젝트 요약입니다. 소스 코드는 공개하지 않았습니다.

### ✨ 주요 기여

- **Fourier peplography 기반 안개 제거** — 공간 주파수 합성을 활용한 물리 기반 영상 복원 알고리즘을 구현하여 대기 산란으로 인한 이미지 손실을 복원했습니다.
- **Photon Counting 기반 저조도 복원** — 저조도 센서 입력으로부터 사용 가능한 영상을 복원하는 광자 계수 파이프라인을 구축했습니다.
- **기기 탑재** — 핵심 로직을 C++/OpenCV로 작성해 Android 네이티브 플러그인(`.so`, arm64)으로 빌드하고, 헤드셋의 Unity(IL2CPP) 앱에서 기기 카메라만으로 동작하도록 연동했습니다.

### 🛠 기술 스택

| 계층 | 기술 |
|---|---|
| **알고리즘** | Fourier peplography, Photon Counting |
| **코어** | C++, OpenCV (Android 네이티브 빌드, arm64) |
| **연동** | Unity (IL2CPP) ↔ Android 네이티브 플러그인(`.so`) |
| **하드웨어** | Metalens 2 XR Headset |

### 🎯 성과

메이커톤 현장에서 XR 헤드셋을 통한 실시간 안개 제거 및 저조도 복원 시연을 성공적으로 진행했으며, 광학 이미징 원리와 실시간 구현 전략을 심사위원 및 업계 참관자에게 발표했습니다.

<div align="right"><a href="#-english">🇺🇸 View in English ↑</a></div>

---

## 📸 Gallery

### On-Stage Technical Presentation / 현장 발표
![presentation](https://github.com/user-attachments/assets/11857cb3-2bbd-4760-a4e6-666ee1d7af74)

