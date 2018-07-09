# Space Explorer

_Space Explorer_ is 3D spaceship-themed game to visualize algorithms. It was initially built by [Yunpeng](https://github.com/yunpengn) in 2016. Since AY2017/2018 Semester 1, it has been used in NUS [CS1101S Programming Methodology](https://www.comp.nus.edu.sg/~cs1101s/) to visualize sorting algorithms and assist CS students to learn programming.

In July 2018, [Yunpeng](https://github.com/yunpengn) has decided to open source it. Although it was originally used to visualize sorting algorithms, it is designed to be open and extensible such that you can do much more than that.

To learn more, you may want to take a look at [the demo video on YouTube](https://www.youtube.com/watch?v=RQTNBPb4Q70).

<div align="center">
	<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/RQTNBPb4Q70?rel=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

## To set up the project

- Unity3D game engine (at least 2017 or newer);
- Git with LFS (large file storage) installed and enabled
	- See the documentation [here](https://git-lfs.github.com/) on how to download and enable Git LFS;
- Change the version control settings in Unity editor
	- Follow the instructions stated [here](https://robots.thoughtbot.com/how-to-git-with-unity).

## To use Git/GitHub with Unity project

Initially, this project is using [Unity Collaborate](https://unity3d.com/cn/unity/features/collaborate) as the version control tool. However, it was deserted soon due to many reasons.

However, using Git (or GitHub) as the version control tool for a Unity project is not as simple as you may think of. This is due to the following reasons:
- **Noise**: The Unity3D editor generated a lot of temporary files just for asssitance purpose. Those files are different for every development machine. Thus, they generally should not be version controller.
- **Unresolvable merge conflicts**: Many files in a Unity project are in binary format. Thus, if you and your collaborator happens to edit the same file _independently_, you could never resolve the merge conflict.
- **Large file size**: Any game project involves a lot of assets (models, sounds, images, etc). However, Git is known to be not good at handling large files. You may want to see GitHub's documentation at [here](https://help.github.com/articles/working-with-large-files/).

Due to the above issues, we have adopted the approach mentioned in this [article](https://robots.thoughtbot.com/how-to-git-with-unity). Basically, there are 3 steps:
- Use a Unity-specific `.gitignore` file;
- Change some settings in Unity editor for version control;
- Use Git large file storage (LFS).

## Licence

[GNU General Public Licence 3.0](LICENSE)
