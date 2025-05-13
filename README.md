# csci-ga3033-090-homework-2-solved
**TO GET THIS SOLUTION VISIT:** [CSCI-GA3033-090 Homework 2 Solved](https://www.ankitcodinghub.com/product/csci-ga3033-090-homework-2-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;93513&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSCI-GA3033-090 Homework 2 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<h2>Introduction</h2>
This homework is designed to follow up on the lecture about Deep Q-Learning. For this assignment, you will need to know about the basics of the deep Q learning algorithm we talked about in class. If you have not already, we propose you brush up on the lecture notes. Furthermore, you will have to learn about a couple of algorithms that we have not discussed in detail in the class: either from the original papers or from blog posts around the internet.

<strong>&nbsp;</strong>Code folder

Find the folder with the provided code in the following google drive folder: <a href="https://drive.google.com/drive/folders/14VehoGYvIiKFJBbGKZdRquTCnlS9J4kv?usp=sharing">https://drive.google.com/drive/folders/14VehoGYvIiKFJBbGKZdRquTCnlS9J4kv?usp=sharing</a>. Download all the files in the same directory, and then follow the instructions in the env_installation.md file, and then complete the drql.py/utils.py/config.yaml files.

Thanks to Denis Yarats for the template for this code.

<h2>Deep Q-learning</h2>
In the class, we learned about the Deep Q-Network (DQN) Learning algorithm, which is considered the first large scale success for any deep reinforcement algorithm. This method is quite dated now, but for a lot of algorithms used today, the roots can be traced back to DQN.

&nbsp;

One of the algorithms improved on DQN is Rainbow (<a href="https://arxiv.org/abs/1710.02298v1">https://arxiv.org/abs/1710.02298v1</a>), which combined some of its contemporary improvements over DQN into one algorithm, like dueling DQN, double DQN, and Prioritized Experience Replay. Finally, more recently, Data-regularized Q-learning (DrQ) has improved on this baseline by adding image augmentations to DQN.

&nbsp;

In this homework, we provide you an example implementation of DQN. We ask you to add some of those improvements made in Rainbow and DrQ to get to an almost state-of-the-art deep RL algorithm.

<h3>Environment</h3>
The environment we will use in this homework is built upon the Pong, Space Invaders, and Breakout environment from OpenAI gym Atari environments (<a href="https://gym.openai.com/envs/#atari">https://gym.openai.com/envs/#atari</a>).&nbsp; In this homework, we will attempt to learn these agents from image observations. We already have a working implementation of DQN on the code folder, which you can run as python train.py env=Breakout and so on. Your job is to complete all the TODOs, and turn on the completed features one by one. You can download the code folder, with every file associated, from here <a href="https://drive.google.com/drive/folders/1T8B3gSNWjQU-JpifHkEDm9FfoxJA6wB_?usp=sharing">https://drive.google.com/drive/folders/1T8B3gSNWjQU-JpifHkEDm9FfoxJA6wB_?usp=sharing</a>

<h3>Question 1</h3>
Download the code folder, and run the code for the three given environments. Make a plot of their performance over time. This is your baseline, and you will compare your future improvements to the code with this baseline to test their validity.

<h3>Question 2</h3>
First, add <a href="https://paperswithcode.com/method/double-q-learning">Double Q-learning</a> onto the model (find the place by searching “TODO: double Q learning” in the code files.) Make another plot by running the three environments on your code that use double Q learning.

<h3>Question 3</h3>
Next, implement Prioritized Experience Replay. In the replay_buffer.py file, we already have an implementation of a prioritized replay buffer. Use that in your code. Find “TODO prioritized replay buffer”, and fix the priority update for the prioritized replay buffer. Make another set of plots, and compare them to the plots from Q2. Is your performance better or worse now? Try explaining your observations.

<h3>Question 4</h3>
Finally, implement <a href="https://towardsdatascience.com/dueling-deep-q-networks-81ffab672751">Dueling DQN</a>. Find the places where you have to put your code by searching for “TODO dueling DQN”. As before, plot your performance in the three environments. Now that you have an almost complete implementation of Rainbow, combine all of your plots together and show the improvement over vanilla DQN.

<h3>Question 5</h3>
<strong>Bonus points</strong>: We still haven’t used DrQ anywhere. Read the code to try and figure out how to use DrQ on top of DQN. You can read more in the blog post by the authors of the original DrQ paper here: <a href="https://sites.google.com/view/data-regularized-q">https://sites.google.com/view/data-regularized-q</a>. You will have to:

<ul>
<li>Figure out what the best data augmentations are for the environment you have,</li>
<li>Add those augmentations into the training process, and</li>
<li>Report (improved) results from using those augmentations.</li>
</ul>
<h2>Python environment installation instructions</h2>
<ol>
<li>Make sure you have conda installed in your system. <a href="https://conda.io/projects/conda/en/latest/user-guide/install/index.html#regular-installation">Instructions link here.</a></li>
<li>Then, get the conda_env.yml file, and from the same directory, run conda env create -f conda_env.yml.</li>
<li>Finally, run the code with python train.py once you have completed some of the to-do steps in the code itself.</li>
</ol>
&nbsp;
