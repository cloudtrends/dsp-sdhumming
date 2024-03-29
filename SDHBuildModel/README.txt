用途

本目录所包含代码及工程用来由MIDI音轨文件创建可被用于检索的库文件。通过使用本目录的代码所生成的工具，用户可以将一组MIDI文件生成检索用的旋律库。假如工具的名字叫做SDHuildModel，那么旋律库的生成是这样的：

	命令行> SDHuildModel.exe mid_list.txt model_dir

其中，mid_list.txt是所有MIDI文件的列表，每行一个MIDI文件的路径，程序可通过此路径找到相应的MIDI文件。该文件采用chinese-iso-8bit编码或GB编码。model_dir是旋律库的输出目录。当程序运行成功之后，该目录下会生成两个文件，分别是QBHModel.dat和QBHModel.info。该库文件稍后可被用于哼唱检索模块（SDHumming）。

有关说明

创建旋律库的主要过程就是从MIDI文件中提取出正确的主旋律的过程。而由于MIDI文件的种类多样，机器并不能100%保证从MIDI音轨中提取出正确的主旋律。本演示程序所附带的旋律库的生成过程经过人工干预，因此当用户使用采集的MIDI文件生成旋律库时，检索效果可能不如前者。鉴于音乐版权问题，恕本软件不附带任何MIDI文件。

版权声明

本目录所包含内容遵守盛大网络哼唱检索开源软件的版权声明。
