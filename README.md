# Release Information

- **Version**: 1.0.0

- **Certified**: Yes

- **Publisher**: Fortinet

- **Scope**: Context and Enrichment, Insight

- **Verified with Models**: Fortinet FortiAI (AI model Medium)

# Impact Analysis Agent

Evaluates threat risk using configurable knowledge and contextual data. Aligns threats with relevant organizational impact scopes and produces structured assessments prioritizing high-risk threats with detailed explanations.

## Installation

This agent installs along with the FortiAI solution pack.

## Configuration

**Required MCP Servers**: NA

<!-- > [!Note]
>
> Refer to [Configuring MCP Servers](https://docs.fortinet.com/document/fortisoar/8.0.0/administration-guide/823139/mcp-servers#Configure_MCP_Servers) on FortiSOAR platform documentation for information on configuring a custom MCP server.
>  -->

### Prerequisites

- The FortiAI solution pack must be installed and configured with the Fortinet FortiAI connector.

  - To configure the FortiAI solution pack, refer to the [FortiAI](https://github.com/fortinet-fortisoar/solution-pack-fortinet-advisor/) solution pack documentation.
  - To configure the Fortinet FortiAI connector, refer to the [Fortinet FortiAI](https://docs.fortinet.com/fortisoar/connectors/fortinet-fortiai) connector documentation.

> [!Note]
>
> FortiAI solution pack and Fortinet FortiAI connector are preconfigured out-of-the-box with FortiSOAR `v8.0.0`.
> 


## Input Parameters

The input must be provided as a JSON object.

| Parameter               | Description                                                                                                       |
|-------------------------|-------------------------------------------------------------------------------------------------------------------|
| `natural_language_task` | Instruction describing how threats should be evaluated using configurable risk knowledge and contextual criteria. |
| `data`                  | Structured contextual data used to compute risk and evaluate threats.                                             |

## Response

The output is returned as a JSON object.

| Parameter | Description                                                                                                                           |
|-----------|---------------------------------------------------------------------------------------------------------------------------------------|
| `status`  | Indicates whether the risk evaluation completed successfully or failed.                                                                       |
| `data`    | Structured output containing evaluated threats, contextual risk assessment, and highest-risk threat identification with explanations. |

