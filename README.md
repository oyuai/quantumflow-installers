### Prerequisites
Before installing QuantumFlow, ensure you have:
- Debian-based Linux distribution
- Root/sudo access
- Working internet connection

## Ubuntu/Debian Based Linux Installation Guide
### Installation Steps

#### 1. Download QuantumFlow
Download the QuantumFlow Debian package from GitHub:

Sign up for Quantumflow here: https://oyu.ai/quantumflow/ and receive instructions to download
<!-- ```bash -->
<!-- dpkg -i ./quantumflow.deb -->
<!-- ``` -->

#### 2. Install the Package
Install the downloaded Debian package using dpkg:
```bash
dpkg -i ./quantumflow.deb
```

## RHEL/CentOS Based Linux Installation Guide

### Installation Steps

#### 1. Download QuantumFlow
Download the QuantumFlow RPM package from GitHub:

Sign up for Quantumflow here: https://oyu.ai/quantumflow/ and receive instructions to download
<!-- ```bash -->
<!-- dpkg -i ./quantumflow.deb -->
<!-- ``` -->

#### 2. Install the Package
Install the downloaded RPM package using the `rpm` command:

```bash
rpm -i ./quantumflow.rpm
```

## Configuration Files
After installation, you'll find two configuration files in `/etc/quantumflow/`:

1. [`app.config.yml` - Main application configuration](../quantumflow-configuration/general-qf-config)
2. [`snmp.yml` - SNMP enrichment configuration](../quantumflow-configuration/snmp-config)

## Starting the Service
To start the QuantumFlow service, run:
```bash
systemctl start quantumflow
```

## Verifying Installation
To verify that QuantumFlow is running correctly:
```bash
systemctl status quantumflow
```


## Troubleshooting
If you encounter any issues during installation:
1. Check system requirements
2. Verify configuration file syntax
3. Review system logs using `journalctl -u quantumflow` OR `cat /var/log/quantumflow/quantumflow.log`
