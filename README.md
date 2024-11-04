# ELK SIEM Lab: VM Log Integration, Visualization, and Alerting

This project demonstrates how to set up an **Elastic Stack (ELK) lab** to monitor logs from virtual machines (VMs), create visualizations, build a dashboard, and set up alerts for system monitoring.

## Project Overview

- **Objective**: Use Elastic Stack to collect logs from VMs, visualize data in custom dashboards, and configure alerts for important events.
- **Tools Used**: Elasticsearch, Kibana, Elastic Agent, Linux VM
- **Description**: Logs from a Linux VM are sent to Elasticsearch with Elastic Agent. Kibana is then used to create visualization, a dashboard, and alerts to monitor key system metrics and events.

## Steps to Set Up

### Step 1: Install Elasticsearch and Kibana
1. Download and install **Elasticsearch** and **Kibana** following Elastic’s installation instructions.
2. Configure basic settings in `elasticsearch.yml` and `kibana.yml` (like network and access settings).
3. Start both services.

### Step 2: Install and Configure Elastic Agent on the Linux VM
1. Install **Elastic Agent** on the Linux VM.
2. Configure Elastic Agent to send system logs directly to Elasticsearch.
3. Confirm logs are being indexed by checking **Kibana > Discover**.

### Step 3: Build a Dashboard
1. **Create a New Dashboard** in Kibana.
   - Add your saved visualizations to display system activity.
2. **Customize the Layout** for easy viewing of important metrics.

### Step 4: Set Up Alerts
1. **Configure Alerts** in Kibana to notify when specific conditions are met, like high CPU usage or repeated errors.
