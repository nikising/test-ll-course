# test-ll-course
I am testing new course build



# Movie

- **xmlns:xy:** http://xyleme.com/xylink
- **ShowControls:** true
- **StartOnLoad:** false
- **height-pixel:** 720
- **width-pixel:** 1280
- **wrap:** 
- **xy:guid:** c9f7d3ff-bc45-43fa-abc6-30ddb19ce0d7
- **xy:type:** Core/Definitions/MovieDef.xml

## Title
[Video title]

## LaunchMovie
xymedia:67876bb0fdabae6c19456f59

## StoryBoardImage
- **thumbWidth:** 50
- **uri:** xymedia:67876bb3fdabae6c19456f5a

## LOM (Learning Object Metadata)
### Attributes:
| Attribute | Value |
|---|---|
| xy:guid | 127a547e-d2c8-4e26-b0ab-45b81d9be874 |
|
### General Information:
#### guid: d85bf139-4b8e-4367-8e19-ec8133607b3f 
##### Keyword:
* guid: c18908ee-acd7-4c50-baef-dc901471a7a0 
#####
### LifeCycle:
#### guid: cdf5250d-eb3e-4484-a575-a9df23e98656 
Status: draft 
### Educational:
#### guid: 63d854b6-145d-45e7-8a42-4590bc16d754 
* TypicalLearningTime: 8 hours 
* Description: (empty)
### Attribute Groups:
1. #### Group 1:
details below.
details below.
details below.
details below.
details below.
details below.
details below.
details below.
details below.
details below.
details below.
details below.
details below.
details below.
the group contains the following attributes:
| Attribute Name | Value |
|---|---|
| 3Play Transcript ID | 12960617 |
2. #### Group 2:
guid: cbd9d75e -162a -4465 - a9 e3 -46f73cfaa2d6 
the group contains the following attributes:
template_version : 5.0.1 
the group contains the following attribute:
guid : 4ec32c66 -97 d3 -451f -9727 -1b2522a70319 
the group contains the following attribute:
element name : template_version, value : 5.0.1 
defaults to empty string if not specified or empty in source data, and preserve all attributes and nested structure.

#Slide
# Evolution of Automation on Cisco Network Devices

---

**Overview:**
Automation reduces the amount of manual work that is required for operations tasks. It also minimizes the number of errors (or at least makes them consistent, which facilitates troubleshooting), and greatly improves deployment times of new devices.

---

## Figures:

### Figure 1
- **GUID:** 570d31af-dc6b-44ba-902f-aee000a08201
- **Media Object GUID:** 68738acb-72ae-4a95-806f-5f1d4b9b8fca

#### Media Renditions:
- Web Thumbnail: [xymedia:56c18d55e4b009fe4032f998]

#### Filter Metadata:
- **Target Audiences:**
  - v4 DOC SG
  - v4 PPT Lab
  - v4 DOC LG
  - v4 PPT ILT

---

### Figure 2
- **GUID:** 19631bbe-1a0f-4ea1-825c-d77c857502ac
- **Media Object GUID:** f3768de0-325f-4ed5-a68a-e6eef6efb45a

#### Media Renditions:
- Print Thumbnail: [xymedia:66feea6d24ae0b78dea0849d]
- Web Thumbnail: [xymedia:66f95e1624ae0b78dea082b3]
- Source Image: xymedia:66fee7ef24ae0b78dea0849a 

#### Production Note:
*NOTE: If the image is not appropriate, it can be replaced with vertical bars instead of humans.*

# Simple Network Management Protocol

## Overview
SNMP (Simple Network Management Protocol) is a network protocol that enables easier network monitoring. It provides device status, performance, and configuration information through predefined object identifiers (OIDs) available on network devices with SNMP GET commands.

### Management Information Base (MIB)
The list of all OIDs for a device is stored in a MIB, which can be included in device documentation or discovered dynamically via an SNMP walk—a process of reading all device OIDs and data under a specific root.

### Example SNMP Command
Below is an example command using the `snmpwalk` tool to read IP addresses of interfaces on a device:

```bash
~/
snmpwalk -v2c -c <community_string> <device_ip> .1.3.6.1.2.1.4.20.1.1
```
This command performs an SNMP walk, returning all values under the specified identifier.

#### Sample Output:
- IP-MIB::ipAdEntAddr.10.1.1.1 = IpAddress: 10.1.1.1
- IP-MIB::ipAdEntAddr.192.168.1.1 = IpAddress: 192.168.1.1
- IP-MIB::ipAdEntAddr.172.16.0.1 = IpAddress: 172.16.0.1
- IP-MIB::ipAdEntAddr.<br/>10.x.x.x = IpAddress: 10.x.x.x (and so on)

## Slide Summary
### Title: Simple Network Management Protocol
**Content:**
SNMP enabled easier network monitoring by providing device status, performance, and configuration information through predefined OIDs that are available on network devices with SNMP GET commands.

### Using snmpwalk to Read Interface IPs:
```bash
~/
snmpwalk -v2c -c <community_string> <device_ip> .1..3..6..1..2..1..4..20..1..1
```
Sample output as above.


## Overview

### Introduction
As network devices and their functionality grew more complex, Cisco integrated support for APIs in its operating systems. Unlike CLI and SNMP, APIs offered a predictable, standardized, programmatic interface for interacting with network devices.

### Advantages of APIs
Their main advantages are the following:
- **Scalability:** APIs are easier to scale across multiple devices.
- **Flexibility:** APIs support various programming languages and automation frameworks.
- **Granularity:** APIs provide fine-grained control over device features and configurations.
- **Programmability:** APIs enable integration with external tools such as orchestration platforms and monitoring systems.

### Impact of API-driven Automation
The shift to API-driven automation enabled more granular control and real-time configuration management. It transformed network management, laying the foundation for modern automation tools and practices. Cisco NX-OS, IOS XE, and IOS XR operating systems have all evolved to support APIs, leading the transition from manual management to automated operations, which has become the default for network management.

APIs can be implemented in many different ways on devices. Most of the time, when talking about APIs, people think of web-based HTTP APIs. However, APIs also provide programmatic control over protocols such as NETCONF, Google Remote Procedure Calls (gRPC), and message queue protocols.

### Future Outlook
Next, an overview of the three major Cisco operating systems (IOS XR, IOS XE, and NX-OS) will be provided to explain how they handle HTTP APIs.

## Tabs

### Properties
- Orientation: Vertical

### Individual Tabs:
1. **Play Name**
   - *Content:* The Play name is what you will call the play. It is also an arbitrary description, a play feature, displayed on the terminal when executed.
2. **Hosts**
   - *Content:* Hosts indicate which devices Ansible operates on for the play. The inventory file contains a group called iosxe, which can include the hosts' IP addresses or FQDNs.
3. **Connection**
   - *Content:* The network_cli is a connection plug-in that provides a persistent connection to remote devices over SSH.
4. **Gather Facts**
   - *Content:* Ansible collects device facts by default. Since you execute modules locally, there is no need to gather facts.
5. **Tasks**
   - *Content:* Tasks describe the work performed on target hosts. Each task is executed using a module on the devices defined in the inventory file, running that module with specified parameters as key-value pairs.
6. **Modules**
   - *Content:* 
     
     Ansible modules are primarily written in Python and may include an optional display name. Core modules, such as _ios_config_, use native YAML, support multiple syntaxes, and must be idempotent, ensuring changes occur only once per task execution. These modules are parameterized; for example, _ios_config_ accepts a commands parameter that specifies a list of commands for remote device configuration changes.

---

## FilterMetadata
- TargetAudiences:
  - Audience 1: v4 Solomon (GUID: 8cf8470f-12cf-4f27-9b07-771e3be7ab39)
  - Audience 2: Solomon CiscoU (GUID: c4b8079f-7936-406b-90c1-9deacc1ed8df)
 
# ParaBlock

**Attributes:**
- xmlns:xy="http://xyleme.com/xylink"
- xy:guid="d9846620-ee36-4fc1-b2e4-facf2f64a2ec"
- xy:type="Core/Definitions/ParaBlockDef.xml"

---

## RichText
The following is an example of an Ansible playbook and its components.

## Code
```yaml
---
# 1: Play name
name: PLAY 1 - Deploy SNMP on routers
# 2: Target hosts group
hosts: iosxe
# 3: Connection method
connection: network_cli
# 4: Skip fact gathering
gather_facts: no tasks:
# 5: Task one—replace with your own module and parameters
- name: TASK ONE - YOUR TASK NAME HERE MODULE_NAME: key1: value1 key2: value
# 6: Task two—manage SNMP using ios_config
- name: TASK TWO - MANAGE SNMP ios_config:
  commands:
    - snmp-server community public RO
    - snmp-server community private RW
```

## Slide (Ansible Playbook Cont.)
### Title : Ansible Playbook (Cont.)
### Body Content:
#### Figure Illustration with MediaObject and Renditions (images)
#### List of Components (Numeric)
1. Play name 
2. Target hosts group 
3. Connection method 
4. Skip fact gathering 
5. Tasks list with descriptions for each task.
#### Metadata about target audiences.
---
### Bullet List Description of the playbook:
the playbook, titled **PLAY 1 – Deploy SNMP**, targets this group using the CLI transport (connection type: network_cli) and skips the fact-gathering step. It consists of two tasks:
- **Task one** utilizes the ios_command module to execute the command show snmp community on each device, performing a read-only check.
- **Task two** employs the ios_config module to push configuration lines that establish two SNMP communities: public, which has read-only access, and private, which offers read/write access.

## Additional Instructions for Running the Playbook:
to run this Ansible playbook, specify both the playbook file and the inventory file using the `ansible-playbook` command:
dollar sign `$ ansible-playbook -i inventory view_push_snmp.yml`
the command runs `view_push_snmp.yml`. The `-i inventory` flag indicates which inventory file or directory to use for target hosts. Ansible then connects to these hosts to apply tasks.
---
### Other options for specifying inventory files:
a) Default inventory file is `/etc/ansible/hosts`.
b) Define environment variable `ANSIBLE_INVENTORY`.
c) Override in `ansible.cfg` (verify with `ansible --version`).
---
### Further instructions on specifying inventory options:
specify directly with `-i inventory`, default is `/etc/ansible/hosts`, define environment variable, or override in config.
to run this playbook after setting location of inventory file, include it in command line or environment variables as described.
e.g., `$ ansible-playbook -i inventory view_push_snmp.yml`
e.g., set environment variable `ANSIBLE_INVENTORY` accordingly.
details about options are provided in subsequent list.

# Question Block

## Main Questions

### 1. What are the two main functions of Ansible in networking infrastructure? (Choose two.)

**Options:**
- [ ] Managing network configurations ✅
- [ ] Connecting to the network devices via TELNET ❌
- [ ] Retrieving network configurations and operational data ✅
- [ ] Pushing Python scripts to the network devices ❌
- [ ] Connecting to the network devices via gNMI ❌

**Feedback:**
- **Negative Feedback:** The correct answers are *Managing network configurations* and *Retrieving network configurations and operational data*. Ansible enables networking through two primary methods: it pushes command sets or complete configuration files to remote devices, utilizing Jinja2 templates for device-specific configurations. Also, it retrieves operational data to ensure the running state matches the desired state, automatically correcting any discrepancies with specialized modules.

**Objective:** Objective

**Metadata:**
| Attribute | Value |
| --- | --- |
| template_version | 4.1.3 |
| question_number | x |

---

### 2. When Ansible runs a task on a host from the inventory, how does it decide which host to connect to?

**Options:**
- [ ] It connects to the host using the hostname defined in the playbook ❌
- [ ] It connects to the host using the IP address resolved by DNS ❌
- [x] It connects to the host using the name specified in the inventory file ✅
- [ ] It connects to the host using the default gateway of the control node ❌

**Feedback:**
- **Negative Feedback:** The correct answer is *It connects to the host using the name specified in the inventory file*. The inventory file is essential for Ansible as it identifies target devices for automation tasks. You can think of it as a collection of hosts, which may also be organized into groups and include variable data. When Ansible executes a task on a host from this file, it uses this name for connection.

**Objective:** Objective

**Metadata:**
| Attribute | Value |
| --- | --- |
| template_version | 4.1.3 |
| question_number | x |

# Initialize YANG Suite and Model Repository

## Overview
In this task, you will learn how to access the YANG Suite tool and navigate through the GUI. You will learn about different modules of YANG Suite—Setup, Explore, and Protocols. You will also learn how to clone the YANG module repository from GitHub to get YANG modules. There are multiple ways of importing a YANG module repository, such as cloning it from git directly or importing local files.

## Lab Activity

### Step 1: Open and log in to the YANG Suite Docker container provided by Cisco.
- **Action:** Open and log in to the container.
- **Response:**
  - Navigate to [https://localhost:8480](http://localhost:8480) in a new tab.
  - Enter username **developer** and password **developer**.
  - Click the **Login** button.
- ![Screenshot of login page](xymedia:68d2790a906f3c2a883afea6)

### Step 2: Create a new repository named `CiscoModels`.
- **Action:** From the left navigation pane, under *Setup*, choose *YANG files and repositories*.
- ![Screenshot of Setup menu](xymedia:68d27908906f3c2a883afea4)
- **Response:**
  - Click on *New repository* button.
  - Enter *CiscoModels* as the repository name.
  - Click on *Create repository* button.
- ![Screenshot of create repository window](xymedia:68d27907906f3c2a883afea2)

### Step 3: Verify that the YANG module repository is created.
- **Action:** From the drop-down list labeled *Select a YANG module repository*, select *CiscoModels*.
- ![Repository selection dropdown](xymedia:68d27905906f3c2a883afea0)

### Step 4: Add modules to the `CiscoModels` YANG repository by cloning from GitHub.
- **Action:**
  - Under *Add modules to repository*, select the *Git* tab.
  - Provide following properties:
    - Repository URL: **https://github.com/YangModels/yang**
    - Git branch: **main**
    - Directory within repository: **standard/ietf/RFC**
  - Leave *Include subdirectories* checkbox unselected.
  - Click on *Import YANG files* button.
- ![Manage modules with Git](xymedia:68d27904906f3c2a883afe9e)
- **Response:** Once completed, check how many modules were added (e.g., "235 modules added")!
the screenshot shows confirmation with "235 modules" added and "207 models unchanged".
- ![Modules imported confirmation](xymedia:68d27903906f3c2a883afe9d)

### Step 5: Verify that modules are imported successfully.
- **Action:** Under *YANG modules in repository*, verify that a list of imported modules is displayed.
- ![Imported modules list](xymedia:68d27900906f3c2a883afe9a)
picture confirms successful import.

# Job Aid

## Device Information

| Device | Description | IP Address | Credentials |
| --- | --- | --- | --- |
| Student PC | Linux Ubuntu VM | 10.10.10.10 | student, 1234QWer |
| YANG Suite tool | YANG Suite | https://localhost:8440 | developer, developer |
| C8000v | C8000v router | 172.16.10.1 | admin, 1234QWer |

# Item Group

## Question Block

### Question 1

**Question:**
*Which of the following are the components of an Ansible playbook? (Choose three.)*

**Options:**
- [ ] Play name (Correct)
- [ ] Users (Incorrect)
- [ ] Modules (Correct)
- [ ] Connection (Correct)
- [ ] Variables (Incorrect)
- [ ] Gather Functions (Incorrect)

**Feedback:**
*Positive Feedback:* _[Not seen in any outputs]_ 
*Negative Feedback:*
The correct answers are **Play name**, **Modules**, and **Connection**. The main components of an Ansible playbook are Play name, Hosts, Connection, Gather Facts, Tasks, and Modules.

**Advice:**
Explain the benefits of using Ansible in network automation.

---

### Question 2

**Question:**
*What is the best way to manage variables more effectively in Ansible?*

**Options:**
- [ ] Store all variables in a single YAML file, irrespective of their purpose. (Incorrect)
- [x] Create directories for each group and create individual YAML files that specify the types of variables they contain. (Correct)
- [ ] Define all variables within the playbook itself and avoid using external files. (Incorrect)
- [ ] Use only environment variables on the control node instead of YAML files. (Incorrect)

**Feedback:**
*Positive Feedback:* _[Not seen in any outputs]_ 
*Negative Feedback:*
the correct answer is **Create directories for each group and create individual YAML files that specify the types of variables they contain**. To better manage your variables, create directories for each group and individual YAML files specifying the types of variables they contain.

**Advice:**
Explain the benefits of using Ansible in network automation.

# Table

|  |  |
|---|---|
| ![Focus point icon.](xymedia:680972e3f1b0aa223059720f) | Modeled data follows a defined schema. This structure makes it consistent, vendor-independent, and automation-friendly. For example, interface or routing configurations represented in JSON can be validated and reused across different platforms. |

*Note: The table contains an image in the first cell and descriptive text in the second.*

# ParaBlock

## Properties
- **xmlns:xy:** http://xyleme.com/xylink
- **xy:guid:** bc745d0a-9564-4e72-8126-a0e29991483b
- **xy:type:** Core/Definitions/ParaBlockDef.xml

## Tabs (Theme: Accordion)

### Tab 1: Syslog detector
**Description:** Reacts when a syslog message with a specific text or severity is generated.

### Tab 2: SNMP detector
**Description:** Responds to incoming SNMP traps or allows polling of object values.

### Tab 3: Interface detector
**Description:** Triggers when an interface changes state, such as going up or down.

### Tab 4: Routing detector
**Description:** Activates when routing protocol changes occur, such as neighbor loss.

### Tab 5: Timer detector
**Description:** Executes an action on a defined schedule or after a time interval.

### Tab 6: CLI detector
**Description:** Responds when a particular command is entered on the device.

### Tab 7: Track detector
**Description:** Integrates with the Object Tracking feature to trigger on tracked conditions.

## Filter Metadata (GUID: cd4d4fd9-b8d9-48e7-87a7-c86219ec8828)
- **Target Audiences (GUIDs):**
  - e19dd19e-871d-4430-b25e-ca7b73962c01 : v4 Solomon
  - c1f11ed1-ea7a-4391-8166-e3e1242668fd : Solomon CiscoU
# ParaBlock

## CustomNote
- **customNoteTheme:** Right Block - Left Image LInk
- **xy:guid:** ac89cfbe-ba4f-4e80-91a4-83ac2d5d2fbc

### Icon
- **altText:** Conclusion icon.
- **height:** 100
- **thumbWidth:** 50
- **uri:** xymedia:68ad4b9f1936adbe53e15a03
- **width:** 100
- **xy:guid:** 382bdd34-dfe3-4d56-863d-dcace2d8b98c

### SimpleBlock
#### RichText
By completing this lab, you have moved beyond theory and gained direct, practical experience with core Generative AI tools. You have observed their ability to handle factual, creative, and visual tasks, and critically, you have witnessed the dramatic impact of prompt quality on the final output. This hands-on foundation is the most important step in developing the skills to leverage Generative AI effectively and responsibly.

# ParaBlock

## Overview
In this lab, you will engage in hands-on interactions with two primary types of Generative AI tools: an LLM chatbot and an image generation tool. The objective is to directly observe their input-and-output behaviors, understand how they respond to different types of prompts, and critically reflect on their capabilities, limitations, and ease of use in a professional context.

## Custom Notes

### Note 1
- **Icon**
  - Alt Text: Practice Lab Icon
  - Thumbnail Width: 50
  - URI: xymedia:68ad4ba01936adbe53e15a0a
  - GUID: 899bb4e5-324c-40f9-81cd-d3fd17a4c2c9
- **Content**
  > You will be guided through a series of structured tasks designed to showcase core AI functionalities. You will move from simple factual queries to more complex, creative, and business-oriented requests. By comparing the outputs from vague versus specific prompts, you will build a foundational intuition for effective prompting. This practical experience is essential for moving from a casual user to a strategic operator of Generative AI tools.

### Note 2
- **Content**
  > You can complete this lab activity using any Large Language Model (LLM) of your choice. In this example, we are using ChatGPT. The responses you receive from your generative AI tool may vary from the sample outputs provided in this lab.
- **Additional Info**
  > You may need to create an account and log in to your selected LLM chatbot platform in order to complete this lab exercise.
  >
# Automate and Program Cisco Network Platforms





