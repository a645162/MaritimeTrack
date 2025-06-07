# MaritimeTrack

MaritimeTrack is a benchmark for tracking multiple objects 

[[Home Page]]()
[[Paper]]()

## Paper

## News

## Dataset

Download the dataset from 
[Hugging Face]()
 or 
[(Recommand) Baidu Drive (code:)]()
 or 
[AliDrive]()
.

If you are a Chinese Researcher, we suggest you to use `Baidu Drive`.

### DanceTrack Format

Organize as follows:

```shell
{MaritimeTrack DanceTrack Format ROOT}
|-- DanceTrack
|   |-- train
|   |   |-- VideoName_SequenceName
|   |   |   |-- img1
|   |   |   |   |-- 00000001.jpg
|   |   |   |   |-- ...
|   |   |   |-- gt
|   |   |   |   |-- gt.txt            
|   |   |   |-- seqinfo.ini
|   |   |-- ...
|   |-- val
|   |   |-- ...
|   |-- test
|   |   |-- ...
|   |-- train_seqmap.txt
|   |-- val_seqmap.txt
|   |-- test_seqmap.txt
|-- TrackEval
|-- tools
|-- ...
```

### LabelMe Original Format

* Notice: You should clone(download) and install [mot-toolkit](https://github.com/a645162/mot-toolkit) first!

Organize as follows:

```shell
{MaritimeTrack LabelMe Format ROOT}
|-- Part Name
|   |-- VideoName
|   |   |-- SequenceName
|   |   |   |-- 00000001.jpg
|   |   |   |-- 00000001.json
|   |   |   |-- ...
|   |   |-- ...
|   |-- ...
|-- ...
|-- *.part.json
|-- ...
```

## Other Projects

[mot-toolkit: A toolkit for Multi-Object Tracking Datasets](https://github.com/a645162/mot-toolkit)
[PicPuzzle: A toolkit to ](https://github.com/a645162/PicPuzzle)

## Citation

If you use MaritimeTrack in your research or wish to refer to the baseline results published here, please use the following BibTeX entry:

```bibtex

```
