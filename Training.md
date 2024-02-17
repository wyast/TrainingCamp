# 未央学术部 Git 训练手册

你好，我是织田信长。现在我来教你如何成为战国乱世中的一方枭雄。为了成为枭雄你肯定需要一个团队，正如我有“织田五大将”；而有了团队就有必要使用 Git。所以，请务必乖乖地跟我学好 Git。  
为了让你信任我，在此放一张帅照。  
<img src="./Nobunaga.jpg">

**在使用训练营之前，确保你已经完成了以下事情：**

1. 阅读了“语雀”上的 Git 入门教程
2. 学会了“狂神说 Git”的内容
3. 通关了 GitHub WorkFlow 训练营
4. 已经成为 GitHub/wyast 公司的成员

    具体的信息都在语雀上。如果你没有打牢基础而来我这儿瞎搞，我会深入而友好地教育你。

## 初始化

#### 目录

打开你的 win Git 或者 Linux，在你喜欢的位置创建你的科协工作目录。

    mkdir wyast
    cd wyast

#### 配置账户

配置你的 Git 账户和密码。注意这里必须是你在 wyast 公司里的账户，否则无法 push。

    git config --global user.name "你GitHub的用户名"
    git config --global user.email "你GitHub的注册用邮箱"

#### 初始化仓库

执行以下命令以获得本训练营的仓库：

    git clone git@github.com:"wyast"/"TrainingCamp".git

执行`ls`命令可以看到出现`TrainingCamp`目录。现在打开此工作目录。

    cd TrainingCamp
    code .

你现在能看到类似这样的右边栏：  
<img src="./code.jpg">

到此处，你已经顺利完成初始化了。

## 写文件

现在需要你写一个文件，这将是你的初阵，作为“合作中你的部分”的模拟。在 FirstBattle 目录下新建一个文件，修改文件名及后缀成为`YourName.cpp`。**YourName 处一律填入你的拼音/英文名/代号/昵称任选其一，不要与他人重复。**  
点击 YourName.cpp，输入以下内容并 ctrl s 保存。

    # include <stdio>

    int main()
    {
    printf("Hello World! I am YourName\n");
    return 0;
    }

## 创建分支并完成 Push

现在你对团队的代码有了自己的贡献，需要把新的代码包推回远端仓库。但是工作时，远端仓库的 main 分支被我织田信长上了锁，避免大家误操作而给团队带来不必要的麻烦。所以，你现在需要 push 到一个分支上，再要求老人们合并。

    git add .
    git commit -m "YourName's first battle !!"
    git push origin main:YourName
