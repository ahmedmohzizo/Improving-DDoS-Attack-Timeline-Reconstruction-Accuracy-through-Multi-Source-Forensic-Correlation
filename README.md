# DDoS Attack Timeline Reconstruction Through Multi-Source Forensic Correlation

## Overview

This project evaluates whether combining multiple forensic data sources improves the accuracy and confidence of Distributed Denial of Service (DDoS) attack timeline reconstruction.

Single-source investigations can provide incomplete visibility and inconsistent timestamps. This lab correlates packet captures, network-security logs, monitoring metrics, dashboards, and written evidence to identify attack phases and validate start and end times.

## Lab Environment

The controlled lab uses three Linux systems:

- **System A - Protected target:** Simulates a secured company database host with restricted administrative access.
- **System B - Test workstation:** Represents a less-restricted host on the same network.
- **System C - Monitoring workstation:** Captures and correlates network and system telemetry.

## Tools

- Wireshark for packet capture and protocol analysis
- Zeek for structured network-security logs
- Grafana Loki for centralized log aggregation and querying
- Prometheus for metrics collection
- Grafana for dashboards and visualization
- Ubuntu and Kali Linux virtual machines
- Python for analysis and supporting workflows

## Investigation Workflow

1. Establish a controlled baseline for network and host activity.
2. Generate authorized DDoS test traffic in the isolated lab.
3. Collect packet captures, Zeek logs, Loki events, and Prometheus metrics.
4. Normalize timestamps and correlate evidence across sources.
5. Compare the reconstructed timeline with known test timestamps.
6. Document attack phases, supporting evidence, and investigation limitations.

## Repository Contents

- `Final report group project/` - final reporting materials
- `Final work steps/` - implementation and investigation workflow
- `Grafana/` - dashboard evidence
- `LOKi/` - log-aggregation evidence
- `Prometheus/` - monitoring evidence
- `Wireshark/` - packet-capture evidence
- `Zeek/` - structured network-log evidence
- `Handshake app/` - supporting application materials
- `Final report project.docx` - full written report

## Key Findings

- Multi-source correlation provides stronger evidence than relying on one telemetry source.
- Cross-source timestamps improve attack-phase identification and validation.
- Packet data, structured logs, and monitoring dashboards provide complementary investigative context.
- Clear evidence organization improves repeatability and post-incident reporting.

## Ethical Use

All attack simulation and monitoring should be performed only in an isolated environment that you own or are explicitly authorized to test.

