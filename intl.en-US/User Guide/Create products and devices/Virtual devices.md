# Virtual devices {#concept_t5p_rqx_w2b .concept}

IoT Platform provides virtual devices to help developers debug devices online. Currently, only Pro Edition supports the online debugging feature.

The general development process of IoT is that, after a device client has been successfully developed, the devices report data to the cloud and developers use the data to develop the applications. Such a development process is often time consuming. In response, IoT Platform provides virtual devices that simulate physical devices connected with the cloud. The virtual devices report defined properties and handle events, and you can debug your applications according to the data reported by the virtual devices. After the physical devices become active, the virtual devices will automatically become inactive.

## Procedure {#section_gbs_tyx_w2b .section}

1.  Log on to the [IoT Platform console](https://partners-intl.console.aliyun.com/#/iot).
2.  In the left-side navigation pane, click Products and then click **View** next to the product that you want to debug.
3.  On the Product Details page, click Online Debugging.
4.  Select the target device to be debugged.

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/17811/154046039510859_en-US.png)

5.  Click **Virtual Device** \> **Start Virtual Device**.

    **Note:** If the physical device is active or disabled, you will be unable to start the virtual device.

6.  Set the content for the simulated push.

    For example, you can set the **Properties**, indoor temperature to be 24 degrees Celsius.

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/17811/154046039510879_en-US.png)

7.  Select a push method.
    -   Push: Only push the data once.
    -   Push Policy:
        -   At Specific Time: Push the data at your specified time.
        -   At Specific Interval: Push the data regularly at your specified time interval in your specified time range. The unit of time interval is in seconds.

You can click **View Data** to view the running status of the device.

If you no longer require a virtual device, click **Stop Virtual Device** to stop it.

## Limits {#section_esp_svd_z2b .section}

-   The minimum time interval for pushing data is 1 second.
-   The maximum number of messages that can be pushed at a specific interval is 1,000.
-   The maximum number of times you can use the Push method per day is 100.

