

# 1.5OLEDBreakout
1.5" OLED Breakout SSD1351

Who doesn't love OLED's? Their relatively low power requirements as well as vibrant color displays are alluring to the hacker. While working on a few projects recently I had the need to interface with one of these OLED displays. There didn't seem to be any breakout boards that broke out the parallel interface pins of the controller, so I decided to make my own.

Scouring the internet for a decent OLED display, I came across this one from buydisplay.com. It's a 128x128 RGB display, with 1.5" diagonal measurement. The controller, SSD1351, supports a 8, 16, or 18 bit parallel interface, as well as SPI for communications. It seemed perfect for the projects I had in mind. Most breakout boards out there only take advantage of the SPI pins of the controller, and at least one of my projects would require access to the parallel interface, so I decided to just build my own board to suite my needs. Hopefully someone else finds it useful.

After tying BS0 and BS1 to ground to enable SPI, I tested the OLED with the [adafruit  SSD1351 driver library](https://github.com/adafruit/Adafruit-SSD1351-library).

![OLED Breakout running test program from Adafruit SSD1351 library](https://lh3.googleusercontent.com/MsKkN0FBhNv1MBZHOAWehuTeS2_8jIe-vTxg2sqLBS44pNBJPy4iuyDUc9Usf4BQjBpzPWWo7Bnqe3NkQCG8paahzHArL8N2OJRp6vAqdoAcOqIph1lTVyudKYCDfX7VTnMsb4jkWHEpYea2pUTW6P7bMah0QvajGr9Vv_Ka1nz8VvwMx_XcXBHSA8MVLC4mheWbWq2etjKzS0w7jgDfSmGsj1dWxFcMfnDJYUARnoZf_Ecu_VUkCVuFhfB3bfooKdvGITS8FaRpiiIor4YhDutwE9h8ZXBRsJ0EaRE9oovJ_CZIdYoFb1mrJiMMzbZo_m1NONMx31lA0AtXVxDD3_TSAVwcc_2xc-_wRHR5UxiRDyMdHFiY_l0dUZIc7PXVY9yiFTdeTccjxLrm2XppLVS5QKP7OgbR_IOFpHCrpZ6-vbgaLmIw-qbnifM7X68Q8axLn03WRp7NhK2jvG_d8vboeV-OaZebjD-bPcUK_6cenOedzorvjP1qjMNFs7BaMNp_RFqAtlz56_IL618pNLowKLZ3Uh-RCuQk9Qy1iAJN5mOoGUT4JS21LYV82Z59FOqgL9iSNJIoaGaWEbZlrih909cDvEl6fb_3MQ4k=w1688-h949-no)

![enter image description here](https://lh3.googleusercontent.com/N4O0tLOCn0Eo37ZxnNt6EblDyE1QjhN_yxB5joiKvIgpHKnZqY0Tt5LPPp8S8s6vpi8v4A9ziG02BMIxa5gTNILQGj3B6yaHgSGacTQC9WjqcnNdZdKckPPqEXiD1Bdt_oRc85JqJZIHr91pL3aQS7A8h610xYnENwIUSkq75CgIYe2bPRbvZ_B09w-lDonRjTYo7xuQ_842ufJOjFXs10Rznar2i5o7Cc5IxF0kcFH1wVu8sHFTCEm_xffTFr8UgDPmG-y94f-umWpQks5XLWrhS6qLWHBYn4ED8aYl1b2wHeDXSp1CXR3UVtDq5sChqppDEJJUfjohhNUl4RfgfJebFzFZR6ZVvmNS3mhxa7NHj9fORLQlyYdXboQTziLBcRMhZDKCvBUCDJ3TQCTlVttUPPMoPq4F5qaboPdrU_tSyGRhDdRTijBlBIn3xsylU8Ip844YMhsJtS_O6xY9tNjXKBb7gK3YVKy-qaMtF4O1Z26QXzV2yLqy29ZDMwsqhQKAy-5qafAfvoEdfoSLm69EmFEEJ4fB6paoH-9Wn0k8a7aUpfmgh1wDXKqv0JxGyFew9EZ3R-GR-hWV9tqFCL4f2KFu_bQE072QgY-5=w1079-h607-no)
