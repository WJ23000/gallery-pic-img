上传到github

git init

git add README.md

git commit -m "first commit"

git remote add origin https://github.com/WJ23000/gallery-pic-img.git

git push -u origin master



生成gh-pages分支步骤：

1、将远程仓库克隆到本地：
git clone https://github.com/WJ23000/gallery-pic-img.git

2、生成分支gh-pages并切换到此分支
cd gallery-pic-img （进入到你克隆仓库的本地文件夹）
git checkout --orphan gh-pages (创建分支并切换)

3、将本地克隆文件(文件名为github仓库名)里面除.git文件以外的其他文件全部删除，再将根目录下dist文件夹里面的内容复制到克隆文件中。
git add . （将本地所有文件加到仓库里）
git commit -m "首次提交" （设置提交信息）
git remote add origin https://github.com/WJ23000/gallery-pic-img.git（本地仓库链接远程仓库）
git push -u origin gh-pages （push文件到仓库中）