# MaritimeTrack

<div align="center">
  <p>
    <a href="https://github.com/a645162/MaritimeTrack" target="_blank">
    <img src="./Resource/Logo/MaritimeTrackLogo.svg" alt="Logo" width="200"/>
    </a>
</p>

<!-- [English](README.md) | [简体中文](README_zh-CN.md) -->

</div>

![](./Resource/separate.png)

MaritimeTrack is a benchmark for tracking multiple objects, specifically designed for maritime scenarios. It provides a comprehensive dataset and standardized evaluation protocols to facilitate the development and comparison of multi-object tracking methods in challenging maritime environments.

<div align="center">

[[Home Page]](https://a645162.github.io/MaritimeTrack/) | [[Github]](https://github.com/a645162/MaritimeTrack) | [[Paper]]()

</div>

## Paper

Comming soon.

## News

More statistics will be coming soon.

## Maritime Dataset

If you are a Chinese Researcher, we suggest you to use `Baidu Drive`.

### All

#### Latest version: v1.0.0(20250322)

<!-- Download the dataset from 
[Hugging Face]()
 or 
[(Recommand) Baidu Drive (code:)]()
 or 
[Aliyun Drive]()
 or 
[Quark Drive]()
. -->

<!-- ![Video Info Sheet (Google Sheets)]() -->
<!-- ![Video Info Sheet (Feishu)]() -->

Comming soon.

### Subset

If you find our full dataset too large, you may consider using the subset we provide.

#### Inland Waterway (River) Subset

##### Latest version: v1.0.0(20250327)

Comming soon.

#### Ocean Subset

##### Latest version: v1.0.0(20250327)

Comming soon.

### DanceTrack Format

The `DanceTrack Format` is compatible with most tracking methods in **recent years**.

Organize as follows:

```shell
{MaritimeTrack (DanceTrack Format) ROOT}
|-- DanceTrack
|   |-- train
|   |   |-- {Video Name}_{Sequence Name}
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
|   |-- train_seqmap.txt # List of sequences
|   |-- val_seqmap.txt
|   |-- test_seqmap.txt
|-- TrackEval
|-- tools
|-- ...
```

For more information on the DanceTrack format, please refer to the [DanceTrack Official Github Repo](https://github.com/DanceTrack/DanceTrack).

### LabelMe Original Format

* Notice: You should clone(download) and install [mot-toolkit](https://github.com/a645162/mot-toolkit) first!

Organize as follows:

```shell
{MaritimeTrack (LabelMe Format) ROOT}
|-- {Part Name}
|   |-- {Video Name}
|   |   |-- {Sequence Name}
|   |   |   |-- 00000001.jpg # Image
|   |   |   |-- 00000001.json # LabelMe Format Annotation
|   |   |   |-- ...
|   |   |-- ...
|   |-- ...
|-- ...
|-- {Spilt config}.part.json # Spilt
|-- ...
```

### MOT Challenge Format

`MOT Challenge Format` is compatible with most of the tracking methods.

We **not directly provide** the `MOT Challenge` format.

Please use `mot-toolkit` to convert to `MOT Challenge` format manually.

The main difference between the `MOT Challenge Format` and the `DanceTrack Format` is that `DanceTrack` uses 8-digit numeric filenames, while `MOT Challenge` uses 6-digit numeric filenames.

### Detection

We not provide the `Detection` format.

Please use `mot-toolkit` to convert to `COCO` or `YOLO` format manually.

## mot-toolkit

[[Github]](https://github.com/a645162/mot-toolkit)

We create a toolkit for `MOT` Dataset.

### Features

* [x] Convert `LabelMe` to `COCO` or `YOLO` Detection format.
* [x] Convert `LabelMe` to `DanceTrack` or `MOT Challenge` or `BDD-100K` MOT format.
* [x] PySide6(Qt) GUI to make annotations.
* [x] Dataset Statistics toolkit
* [x] SAM2(Segment Anything Model 2) to fix bbox.
* [ ] SOT(VOT) method to assist MOT annotation.

## Other Projects

[mot-toolkit: A specialized toolkit for constructing and analyzing multi-object tracking datasets](https://github.com/a645162/mot-toolkit)

[PicPuzzle: A puzzle tool that supports mixed arrangement of landscape and portrait pieces](https://github.com/a645162/PicPuzzle)

<!-- ## Citation

If you use `MaritimeTrack` in your research, find our work helpful, or wish to reference the baseline results published here, please consider citing our work using the following BibTeX entry:

```bibtex

```

**Only for Chinese users:**

同时，我们提供`国标GB／T7714-2015`格式的引用:

```txt

``` -->

## Other Datasets

### Singapore Maritime Dataset (SMD)

Comming soon.

## Related Works

[Singapore Maritime Dataset (SMD)](https://github.com/tilemmpon/Singapore-Maritime-Dataset-Frames-Ground-Truth-Generation-and-Statistics)

## Create your own dataset

Please refer to [mot-toolkit](https://github.com/a645162/mot-toolkit).

## Authors

### Haomin Kong (孔昊旻)

**Notice:**
* If you have any questions, please report them **use the GitHub Issues**!

[[GitHub: @a645162]](https://github.com/a645162)
[[E-Mail: a645162@gmail.com]](mailto:a645162@gmail.com)

## Contribution

To report an issue use the GitHub issue tracker. Please provide as much information as you can.

Contributions are always welcome. Open an issue to contact me. The preferred method of contribution is through a github pull request.
