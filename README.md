# SampleRateConverter
A simple audio sample rate converter

# 说明
- 这是一个基于相似三角形性质的近似采样率转换算法，可以将任意采样率的音频转换成其他任意的采样率，能用在精度不高，但需要处理速度快的场合。
- 此算法处理的结果在低频范围内的频率分布基本和Cool Edit软件处理的效果一致，但高频部分可能有损失。
- 由于只用直线估计实际采样点之间的采样值，没有滤波过程，此算法的时间复杂度只有O(n)。
- 在我的PC上运用此算法，3分钟的音频文件从44.1K转到48K只需处理1秒左右；而同一环境下，Cool Edit需要处理近半分钟。
- wav文件读写的类来源于[这里](https://github.com/sintrb/WaveAccess/tree/master/src/com/sin/java/waveaccess)

# Description
- This is an approximate sampling rate conversion algorithm based on similar triangular properties. It can convert any sample rate audio into any other sampling rate, which can be used in situations where the precision is not high but the processing speed is fast.
- The result of this algorithm is that the frequency distribution in the low frequency range is basically the same as that of the Cool Edit software, but the high frequency part may be lost.
- Since only the straight line is used to estimate the sampling value between the actual sampling points, there is no filtering process. The time complexity of this algorithm is only O (n).
- In my PC using this algorithm, 3 minutes of audio files from 44.1K to 48K only need to deal with about 1 second; and the same environment, Cool Edit need to deal with nearly half a minute.
- Wav file read and write classes are from [here](https://github.com/sintrb/WaveAccess/tree/master/src/com/sin/java/waveaccess)
