---
sidebar_position: 3
---

# CompuTec Gateway Manager

Here you can find a step-by-step guide on how to configure CompuTec WeightScale manager.

---

## Prerequisites

- Configure your firewall to make the 8080 port available

- Net Framework 4.7 is required

## Installation

1. The application is installed automatically during CompuTec Gateway Service installation.

2. Go to the WeightScale configuration manager installation folder and run the file WeightScaleConfigurationManager.

   It is located in an installation folder, which is by default in the following location: C:\Program Files (x86)\CompuTec\CompuTec Weight Service\.

   ![Installation folder](./media/computec-gateway-manager/installation-folder.png)

3. Click Add to add a new weighting device with a unique identifier.

![Add new scale](./media/computec-gateway-manager/add-new.png)

4. Available Scales tab columns:

- **Id** – a unique identifier of the scale (automatically generated)

- **Scale name** – the name of the weighting device (e.g. manufacturer)

- **Localization** – location of the device (check a [related PDC Settings option](../setting-up-the-application/pdc-settings/pdc-settings.md#assigning-pdc-settings-templates))

- **Barcode** – a barcode or a serial number of the device

- **Tolerance** – weight tolerance

- **Range From** – weighing range (start)

- **Range To** – weighing range (end)

- **Session Life Time** – inactive session time (seconds)

  ![Scales columns](./media/computec-gateway-manager/scales-columns.png)

5. Once you click the scales identifier, the setup window opens in the Parameters tab.

![Scale parameters](./media/computec-gateway-manager/scale-parameters.png)

6. Expand the driver tab to select an available device. There are two possibilities to connect the weight scale:

   a. TCP/IP – enter the IP address and port of the scale (the default port number is 4305).

   ![Scale IP](./media/computec-gateway-manager/scale-ip.png)

   b. RS232 – you can change COM port, parity, baud rate, handshake, data bits, stop bits, and regular expression.

   ![Scale RS232](./media/computec-gateway-manager/scale-rs232.png)

7. Now you can save the configuration and perform a test of the printer. Remember to put the Web Address. (It is required to put the IP address or a machine name of the server where Service Layer is installed). The default port is 8080. You can change the port number if needed.

<details>
  <summary>Click here to check how to change the port</summary>
  <div>
    The port can be changed by editing a file located in CompuTec Service Layer installation folder. The default path: C:\Program Files\CompuTec\CompuTec Service Layer\CompuTec.ServiceLayer.Host.WindowsService.exe

    ![Port config](./media/computec-gateway-manager/port-config.png)

  </div>
</details>

:::warning

The address and port in the [corresponding CompuTec PDC Setting](./../setting-up-the-application/setting-up-the-application.md#ct-labels-settings) must be identical to those entered here.

:::

![Manager](./media/computec-gateway-manager/manager-1.png)

![Manager](./media/computec-gateway-manager/manager-2.png)
