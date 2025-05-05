# StreamingInterviewTask
# CDC Pipeline Implementation

A Delta Lake-based Change Data Capture (CDC) pipeline that processes Salesforce Opportunity data in both batch and streaming modes with Unity Catalog integration.

## Overview

This implementation provides:
- Batch and Streaming CDC processing
- Delta Lake integration
- Change tracking and audit logging
- Unity Catalog governance

## Architecture

### Data Flow
```plaintext
Source Data (Salesforce)
      ↓
Streaming/Batch Ingestion
      ↓
Delta Lake Tables (Main + Changelog)
      ↓
Unity Catalog (Governance Layer)
