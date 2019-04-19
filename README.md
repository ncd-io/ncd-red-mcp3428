This library provides a class for the MCP3428, it relies on the ncd-red-comm library for communication, and includes a node-red node for MCP3428. The MCP3428 is a 4-Channel Analog to Digital Converter with 16-Bit resolution, ideally suited for low-speed high-resolution sensor monitoring. [Ncd.io](https://ncd.io) manufactures a multiple easy to use form factors that utilize this converter. You can view list of available boards [here](https://store.ncd.io/?fwp_product_type=analog-to-digital-converter&fwp_chip_name=mcp3428).

[![MCP3428](./MCP3428.png)](https://store.ncd.io/?fwp_product_type=analog-to-digital-converter&fwp_chip_name=mcp3428)

### Installation

This library can be installed with npm with the following command:

```
npm install ncd-red-MCP3428
```

For use in node-red, use the same command, but inside of your node-red directory (usually `~./node-red`).

### Usage

The `test.js` file included in this library contains basic examples for use.  All of the available configurations are available in the node-red node through the UI.

### Raspberry Pi Notes

If you intend to use this on the Raspberry Pi, you must ensure that:
1. I2C is enabled (there are plenty of tutorials on this that differ based on the Pi version.)
2. Node, NPM, and Node-red should be updated to the latest stable versions. If you skip this step the ncd-red-comm dependency may not load properly.
