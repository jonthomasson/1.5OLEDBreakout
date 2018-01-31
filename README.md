
# 1.5OLEDBreakout
1.5" OLED Breakout SSD1351

Who doesn't love OLED's? Their relatively low power requirements as well as vibrant color displays are alluring to the hacker. While working on a few projects recently I had the need to interface with one of these OLED displays. There didn't seem to be any breakout boards that broke out the parallel interface pins of the controller, so I decided to make my own.

Scouring the internet for a decent OLED display, I came across this one from buydisplay.com. It's a 128x128 RGB display, with 1.5" diagonal measurement. The controller, SSD1351, supports a 8, 16, or 18 bit parallel interface, as well as SPI for communications. It seemed perfect for the projects I had in mind. Most breakout boards out there only take advantage of the SPI pins of the controller, and at least one of my projects would require access to the parallel interface, so I decided to just build my own board to suite my needs. Hopefully someone else finds it useful.

After tying BS0 and BS1 to ground to enable SPI, I tested the OLED with the [adafruit  SSD1351 driver library](https://github.com/adafruit/Adafruit-SSD1351-library).

![OLED Breakout running test program from Adafruit SSD1351 library](https://lh3.googleusercontent.com/y4ClTLt4kAX8JY1dKa6sqs7vdYiofKGVTie4jn05ViLuXUgRtfliAkvOQJpFIHKcxbY5IMfaXAFJBssHu1E88YOobrSxGxJNTLpL0vp6Zd6FlKBXTo66tCligUWRmpi4B-y3I1IG1mRnOPmSMy1saUY_TC6bhmHcT097Y_9XeMewFZ6gIpO0dHUi8202Tj8GK1nLAiKfaPo9id4H8oyBSnGFJolL1EJjttHMiJUVCb-rYyqxYrRq-1DkzXndbePQ2UB7_a3rNHXMVxm9ckazghD_cso4vzfK0zZiqWSPPlbHIqk4VLP70oqA0YUMicrwR6aCFZNmCf0xLnEaA2TOq5fg2tcWwUYV6lFBXaj-i0VX0AKvYsrpO4njbEx_Fc5QV9GlqZ1m3qw9et5-l_-75v5WtyyH-voDqTXSWaypxpCvmOQn6aRz6hso7l0ZJA7IMqYpJdn8nc4jl7tD_1Vy_iXxlzS0GhvjnlnNiUe1VF_73AkG9gy7djEWCmAo503nMlJnyAu_ZKygwwvjtXJX9rwIkJqwH1QLG1kzK3Qn45Fj8wCG1L35cVAAhO7uHmXZC_s8sjkL9HtpOOVGZzgroxAuKkO6G_ZH3xS-sGTg=w1593-h896-no)

![enter image description here](https://lh3.googleusercontent.com/-B1VwuNGP_oVGeokW5yNua7Uwk_GOHUQ-a7_rTr_LLlmMEMnIyNNJyLEC6jLQVITlAVFbcPvY-d624zXE4eXg5nT62KSzlZs-x5InFcdZ_FhgpJNtx2LMruzGjloyXw7KTZnGbhl0bVoa2aUihJYIPIan1Z8IdJCgQqW2o66N_iH0RKfnyD_ygSy2jAL1SDV-coDXztDh2Gpq-Vo06QErfVKmyVuH8G53OT-IdVPD8a57pBSAhLBMr2J6WB-4DmKUK7pcNl5LT2Y6kupZOxdxqCw33N6k7p0JEkdP9EJnaTSIk9_0-WRweL0MLa0Wi7HjzSEvoDm1cytKu38UbAihoSLUs_KZG2uACYKIyiXBc3vycIrxmZ4W6IwE6F72Lj9W4ZTy8MlSsTH6dSg7qg3Y_-xC4QLetxEPC-OFVBWDnWha1vqngL6e7ANnlKCtb0OMPIqSl0tUmcVyk2YC419pAYzbw4os3DQrjgrZqF40iGzUforswi1yjy2V0KNi-IDo-JP1dZa6X_vCOhCjx0O8GJWgkyQJpdpsK-5o2nZDWBQhAODxdoaToZ6FSVIev3QxRXN31a4a4fnWDic4SRXFnXeNEJoh7YZEt-nBcFR=w1593-h896-no)
