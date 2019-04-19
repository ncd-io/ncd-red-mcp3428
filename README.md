This library provides a class for the MCP3425, it relies on the ncd-red-comm library for communication, and includes a node-red node for MCP3425. The MCP3425 is a 1-Channel Analog to Digital Converter with 16-Bit resolution, ideally suited for low-speed high-resolution sensor monitoring. [Ncd.io](https://ncd.io) manufactures a mini-module that utilizes this converter in an easy to use form factor. You can view and purchase the mini-module [here](https://store.ncd.io/product/mcp3425-16-bit-1-channel-analog-to-digital-converter-i2c-mini-module).

[![MCP3425](./MCP3425.png)](https://store.ncd.io/product/mcp3425-16-bit-1-channel-analog-to-digital-converter-i2c-mini-module)

### Installation

This library can be installed with npm with the following command:

```
npm install ncd-red-mcp3425
```

For use in node-red, use the same command, but inside of your node-red directory (usually `~./node-red`).

### Usage

The `test.js` file included in this library contains basic examples for use.  All of the available configurations are available in the node-red node through the UI.

### Raspberry Pi Notes

If you intend to use this on the Raspberry Pi, you must ensure that:
1. I2C is enabled (there are plenty of tutorials on this that differ based on the Pi version.)
2. Node, NPM, and Node-red should be updated to the latest stable versions. If you skip this step the ncd-red-comm dependency may not load properly.
