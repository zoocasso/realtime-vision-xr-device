<div align="center">

# 🥽 Real-Time Vision Enhancement for XR Headset

**2024 Pangyo XR Device Makerthon — Sole Developer**

[![EN](https://img.shields.io/badge/Language-English-blue?style=flat-square)](#-english)
[![KR](https://img.shields.io/badge/언어-한국어-red?style=flat-square)](#-한국어)

</div>

---

## 🇺🇸 English

A wearable real-time vision enhancement system for the **Metalens 2 XR headset**, designed to restore visibility in fog and low-light conditions through optical-imaging algorithms deployed on embedded ARM64 hardware.

### 📋 Project Overview

An end-to-end XR vision enhancement pipeline that addresses two critical failure modes of outdoor wearable displays: atmospheric scattering (fog) and photon starvation (low-light). The system targets disaster response, nighttime driving, and industrial inspection scenarios where visual impairment directly affects user safety.

- **Event:** 2024 Pangyo XR Device Makerthon
- **Role:** Sole developer — concept, algorithm implementation, C++/Unity integration, on-stage presentation
- **Target Device:** Metalens 2 XR Headset (ARM64)

### ✨ Key Contributions

- **Fourier Ptychography for Dehazing** — Implemented a physics-based image recovery algorithm that leverages spatial-frequency synthesis to remove scattering artifacts caused by atmospheric haze.
- **Photon Counting for Low-Light Recovery** — Built a photon-counting pipeline that reconstructs usable imagery from photon-starved sensor input, enabling object recognition in near-dark environments.
- **Real-Time Embedded Deployment** — Ported the C++ core into a Unity-loadable DLL targeting ARM64, keeping end-to-end latency low enough for XR headset use without perceptible motion-to-photon lag.

### 🛠 Tech Stack

| Layer | Technology |
|---|---|
| **Algorithms** | Fourier Ptychography, Photon Counting |
| **Core** | C++ (cross-compiled to ARM64) |
| **Integration** | Unity (C# ↔ native DLL) |
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
- **역할:** 1인 개발 — 기획, 알고리즘 구현, C++/Unity 연동, 현장 발표
- **타겟 하드웨어:** Metalens 2 XR Headset (ARM64)

### ✨ 주요 기여

- **Fourier Ptychography 기반 안개 제거** — 공간 주파수 합성을 활용한 물리 기반 영상 복원 알고리즘을 구현하여 대기 산란으로 인한 이미지 손실을 복원했습니다.
- **Photon Counting 기반 저조도 복원** — 광자 부족 환경의 센서 입력으로부터 사용 가능한 영상을 재구성하는 광자 계수 파이프라인을 구축하여 암조도에서도 사물 식별이 가능하도록 했습니다.
- **실시간 임베디드 배포** — C++ 코어를 ARM64 타겟 Unity 네이티브 DLL로 포팅하여, XR 헤드셋에서 motion-to-photon 지연을 체감할 수 없는 수준으로 유지했습니다.

### 🛠 기술 스택

| 계층 | 기술 |
|---|---|
| **알고리즘** | Fourier Ptychography, Photon Counting |
| **코어** | C++ (ARM64 크로스 컴파일) |
| **연동** | Unity (C# ↔ native DLL) |
| **하드웨어** | Metalens 2 XR Headset |

### 🎯 성과

메이커톤 현장에서 XR 헤드셋을 통한 실시간 안개 제거 및 저조도 복원 시연을 성공적으로 진행했으며, 광학 이미징 원리와 실시간 구현 전략을 심사위원 및 업계 참관자에게 발표했습니다.

<div align="right"><a href="#-english">🇺🇸 View in English ↑</a></div>

---

## 📸 Gallery

### On-Stage Technical Presentation / 현장 발표
![presentation](https://github.com/user-attachments/assets/11857cb3-2bbd-4760-a4e6-666ee1d7af74)

### Event Poster / 행사 포스터
<img src="https://github.com/user-attachments/assets/ea51f367-350c-418c-b446-f47464f432b6" width="400" />
