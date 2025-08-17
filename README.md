# Azure Enterprise Cloud Migration Project

## Overview

This repository contains a comprehensive 5-part hands-on Azure cloud migration project designed for IT professionals with system administration experience. The project simulates a real enterprise migration scenario using TechCorp Manufacturing as a fictional company migrating their legacy infrastructure to Microsoft Azure.

## Project Objectives

- **Learn enterprise-grade migration assessment and execution**
- **Master Azure Portal-based migration tools and services**
- **Gain practical experience with real applications and databases**
- **Understand migration challenges and troubleshooting techniques**
- **Develop skills applicable to Azure certifications (AZ-104, AZ-305)**

## Target Audience

- **IT Professionals** with 5+ years of system administration experience
- **Azure certification candidates** preparing for AZ-104 or AZ-305 exams
- **Enterprise architects** planning cloud migration strategies
- **Students and instructors** seeking hands-on Azure migration experience

## Prerequisites

### Required Knowledge
- Windows Server administration experience
- Basic networking concepts (TCP/IP, DNS, firewalls)
- SQL Server database fundamentals
- IIS and web application concepts
- Azure Portal navigation basics

### Required Azure Resources
- **Azure subscription** with Contributor role permissions
- **Estimated cost:** $50-100 for complete 5-part project
- **Regions supported:** US East, US West, Europe West (tested)

### Software Requirements
- **RDP client** for Windows VM access
- **Web browser** (Edge, Chrome, Firefox)
- **Hyper-V enabled** (for local appliance deployment)
- **Internet connectivity** with public IP access

## Project Architecture

### Legacy Environment (Source)
```
TechCorp Manufacturing Legacy Infrastructure:
├── Web Server (techcorp-webserver-legacy)
│   ├── Windows Server 2016
│   ├── IIS with ASP.NET 4.8
│   └── TechCorp Manufacturing ERP Application
├── Database Server (techcorp-dbserver-legacy)
│   ├── Windows Server 2016
│   ├── SQL Server 2019
│   └── TechCorpDB with sample business data
└── Network Configuration
    ├── Public IPs for external access
    ├── NSG rules for required ports
    └── Firewall configuration for services
```

### Target Environment (Azure)
```
Migrated Azure Infrastructure:
├── Azure App Service (Web Application)
├── Azure SQL Database (Migrated Database)
├── Azure Storage Account (File Storage)
├── Azure AD (Identity Integration)
└── Azure Monitor (Monitoring & Optimization)
```

## Part-by-Part Project Breakdown

### Part 1: Migration Assessment using Azure Portal
**Duration:** 6-8 hours  
**Focus:** Portal-based assessment and discovery

- **Environment Setup:** Deploy legacy infrastructure VMs
- **Application Installation:** Complete SQL Server and IIS setup with real applications
- **Azure Migrate Configuration:** Appliance deployment and server discovery
- **Assessment Execution:** Database, web app, and infrastructure assessments
- **Report Generation:** Export and analyze migration readiness reports

**Key Deliverables:**
- Fully functional legacy environment
- Complete migration assessment reports
- Cost estimates and sizing recommendations
- Migration readiness status for all components

### Part 2: Database Migration using Azure Database Migration Service Portal
**Duration:** 4-6 hours  
**Focus:** Azure Database Migration Service

- **DMS Setup:** Portal-based service configuration
- **Schema Migration:** Database structure migration
- **Data Migration:** Full data transfer with minimal downtime
- **Cutover Process:** Production switchover procedures

### Part 3: Application Migration using Azure App Service Migration Assistance Portal
**Duration:** 4-6 hours  
**Focus:** Azure App Service migration

- **App Service Creation:** Portal-based service setup
- **Application Migration:** Code and configuration transfer
- **Connection String Updates:** Database connectivity configuration
- **Testing and Validation:** Application functionality verification

### Part 4: Storage and Identity Migration via Portal Interfaces
**Duration:** 4-6 hours  
**Focus:** Supporting services migration

- **Azure Storage Setup:** File storage migration
- **Azure AD Integration:** Identity service configuration
- **Security Configuration:** Access controls and permissions
- **Hybrid Connectivity:** On-premises integration if needed

### Part 5: Final Optimization, Security Hardening, and Production Readiness
**Duration:** 4-6 hours  
**Focus:** Post-migration optimization

- **Azure Monitor Setup:** Comprehensive monitoring configuration
- **Performance Optimization:** Resource sizing and configuration tuning
- **Cost Optimization:** Resource efficiency improvements
- **Disaster Recovery:** Backup and recovery configuration

## File Structure

```
├── Part1-Migration-Assessment/
│   ├── Part1-Complete-Guide.md
│   ├── SQL-Database-Scripts/
│   ├── Web-Application-Files/
│   └── Troubleshooting-Guide.md
├── Part2-Database-Migration/
│   ├── Part2-DMS-Guide.md
│   └── Database-Migration-Scripts/
├── Part3-Application-Migration/
│   ├── Part3-AppService-Guide.md
│   └── Application-Configuration/
├── Part4-Storage-Identity/
│   ├── Part4-Storage-Guide.md
│   └── Identity-Configuration/
├── Part5-Final-Optimization/
│   ├── Part5-Optimization-Guide.md
│   └── Production-Readiness-Scripts/
├── Resources/
│   ├── Network-Configuration/
│   ├── Sample-Data/
│   └── Templates/
└── README.md
```

## Key Features

### Portal-First Approach
- **100% GUI-based instructions** with minimal command-line usage
- **Click-by-click navigation** with exact button names and menu locations
- **Visual verification** at every step with expected outcomes
- **Portal-native troubleshooting** using built-in diagnostic tools

### Real-World Applications
- **Complete TechCorp Manufacturing ERP system** with ASP.NET 4.8
- **Functional TechCorpDB database** with realistic business data
- **Enterprise networking configuration** with proper security rules
- **Authentic migration challenges** and practical solutions

### Comprehensive Troubleshooting
- **MFA authentication workarounds** for migration tools
- **Network connectivity solutions** for tool access
- **Application compatibility resolutions** for migration issues
- **Performance optimization** techniques and best practices

## Getting Started

### Quick Start (Part 1)
1. **Clone or download** this repository
2. **Open Part1-Complete-Guide.md** for detailed instructions
3. **Follow prerequisites checklist** to ensure environment readiness
4. **Begin with Azure Migrate project creation** following step-by-step guide
5. **Complete all Part 1 objectives** before proceeding to Part 2

### Prerequisites Checklist
- [ ] Azure subscription with appropriate permissions
- [ ] Hyper-V enabled on local machine (for appliance deployment)
- [ ] Public IP identified for NSG configuration
- [ ] RDP client available for VM access
- [ ] Estimated 6-8 hours available for Part 1 completion

## Common Issues and Solutions

### Authentication Challenges
- **MFA with migration tools:** Use Service Principal or Azure CLI device code authentication
- **Legacy tool compatibility:** Disable IE Enhanced Security Configuration when needed
- **Token expiration:** Refresh authentication tokens during long migration processes

### Network Connectivity
- **NSG configuration:** Ensure all required ports are open for external tool access
- **Public IP access:** Verify tools can reach Azure VMs from external locations
- **Firewall rules:** Configure Windows Firewall for SQL Server and web services

### Application Dependencies
- **SQL Server setup:** Complete installation with mixed authentication mode
- **IIS configuration:** Install ASP.NET 4.8 and configure applications properly
- **Service connectivity:** Test all services before beginning migration assessment

## Learning Outcomes

Upon completion of this project, participants will be able to:

- **Plan and execute** enterprise Azure migrations using Portal-based tools
- **Assess migration readiness** for complex applications and databases
- **Configure Azure services** for production workloads using GUI interfaces
- **Troubleshoot migration issues** using practical, proven techniques
- **Optimize costs and performance** of migrated Azure resources
- **Implement monitoring and governance** for migrated environments

## Cost Management

### Estimated Costs (5-Part Project)
- **Virtual Machines:** $40-60 (2 Standard_B2s VMs for 5 parts)
- **Azure SQL Database:** $15-25 (Basic tier for testing)
- **App Service:** $10-15 (Basic tier)
- **Storage and Networking:** $5-10
- **Total Estimated Cost:** $70-110

### Cost Optimization Tips
- **Deallocate VMs** when not actively using them
- **Use Basic service tiers** for learning environments
- **Clean up resources** immediately after project completion
- **Monitor spending** daily through Azure Cost Management

## Support and Contributing

### Getting Help
- **Review troubleshooting sections** in each part guide first
- **Check common issues** documentation for known solutions
- **Verify prerequisites** are met before reporting issues
- **Include specific error messages** when seeking assistance

### Teaching and Training
- **Instructor guides** included with detailed explanations for each decision
- **Business justifications** provided for all technical choices
- **Student exercises** and verification checkpoints throughout
- **Scalable approach** suitable for individual or classroom use

## License and Usage

This project is designed for educational and training purposes. The included sample applications and data are fictional and intended solely for learning Azure migration techniques.

**Recommended Use:**
- Professional development and certification preparation
- Corporate training programs
- Educational institution coursework
- Individual skill development
