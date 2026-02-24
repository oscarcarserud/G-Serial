# G-Serial
A simple serial sender for USB and GRBL

<img width="934" height="654" alt="image" src="https://github.com/user-attachments/assets/90b3cc4d-a586-4a26-9b3b-4ea9f128e020" />

G-Sender works smoothly with pendants connected via TX/RX and does not get confused if the pendant is active. However, please make sure the pendant is monitoring the status. If the status is not “Idle,” I recommend not pressing RUN.

The purpose of this sender is to control program execution, not jogging or other machine settings. You can send those commands, but you would need to send them as separate program snippets.

When you first start G-Serial, connect your Arduino (or other hardware that supports GRBL v1.1h or higher). Then click the [on] button next to “Connect.”

You will now see a list, ideally containing only one selectable device – your GRBL device. Select it.

If you need to change the baud rate from the default 38400 (await port.open({ baudRate: 38400 });) – which is hard-coded – you must modify the code (remember, this is version 0.5).

Once connected, you can paste your G-code into the interface for transmission. Use the large text field on the right for your code.
