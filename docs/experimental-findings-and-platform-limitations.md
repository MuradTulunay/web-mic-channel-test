# Experimental Findings and Platform Limitations

## Overview

This document summarizes experimental observations on microphone input behavior across platforms.

## Key Findings

- Bluetooth headsets expose mono microphone input.
- Some Windows devices report 2 channels but provide highly correlated signals.
- iOS Web APIs do not expose channelCount.
- Web Audio channelCount does not guarantee independent input.

## Critical Insight

Multi-channel availability does not guarantee independent directional data.

## Conclusion

Directional speech admission requires raw multi-channel input, which is not reliably exposed in consumer platforms.
