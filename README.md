# fastq_stat
A fast utility for fastq statistic with Q20/Q30/GCcontent.

### 文件说明

+ kseq.h 源码来源[https://github.com/lh3/seqtk]

+ parse.c 源码来源[https://www.cnblogs.com/xudongliang/p/6397627.html]（结果输出作了调整）

### 使用说明
```
git clone https://github.com/Qian-Kun/fastq_stat.git
cd fastq_stat
gcc -o fastq_stat parse.c -lz

./fastq_stat Sample.fq.gz
```

### 示例
```
$ ${fastq_stat_src_path}/fastq_stat test.fq.gz

TotalReads  TotalBases  Q20bases  Q20pct(%) Q30bases  Q30pct(%) GCbases   GCpct(%)
726942      36347100    35612960  97.98     34728013  95.55     18910391  52.03

```
