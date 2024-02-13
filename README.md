# The Erdős Institute: Deep Learning 
### Spring 2024

Welcome! This is the repo we will be using for the self-paced deep learning course. You will be learning from two sources: <a href="https://www.amazon.com/Deep-Learning-PyTorch-Eli-Stevens/dp/1617295264" target="_blank">Deep Learning with PyTorch</a> and <a href="http://github.com/fastai/fastbook" target="_blank">FastAI's main book</a>.
To learn the material well, you will also meet regularly with a team, who will serve as a study group and a project team. You can form your group on our course page, under "Project/Homework Instructions".

**To get a Deep Learning certificate, you must complete a project by _May 3, 2024_**.

Please note that all of the Jupyter notebooks are based on the content in Jeremy Howard and Sylvain Gugger's <a href="http://course.fast.ai/" target="_blank">fastai course</a> and corresponding <a href="http://github.com/fastai/fastbook" target="_blank">fastai book</a>.

The copyright of the fastai material is:
```
@book{
    howard2020deep,
    title={Deep Learning for Coders with Fastai and Pytorch: AI Applications Without a PhD},
    author={Howard, J. and Gugger, S.},
    isbn={9781492045526},
    url={https://books.google.no/books?id=xd6LxgEACAAJ},
    year={2020},
    publisher={O'Reilly Media, Incorporated}
}
```

The notebooks in this repo are summaries I created of the fastai content in order to consolodate the material and serve as a good review.

## Schedule

This is a self-paced program, but it is suggested to take 12-15 weeks to go through the material. The way the course will work is the following:
1. You will read through the corresponding <a href="http://github.com/fastai/fastbook" target="_blank">fastai chapters</a> and <a href="https://www.amazon.com/Deep-Learning-PyTorch-Eli-Stevens/dp/1617295264" target="_blank">Deep Learning with PyTorch</a> for a particular week on your own.
2. You will meet with your team to have weekly discussions based on the assigned readings. Those meeting will be used to ask each other questions and to spark discussion about applications of deep learning in data science careers.
3. Concurrently, you will be working with your team on a deep learning project of your choosing.

The weekly schedule is below.

Week | Deep Learning Fundamentals | Learning PyTorch
:-------------: | :-------------: | :-------------: 
1 | What is Deep Learning? <br> *fastbook ch. 1* | PyTorch Overview & Tensors <br> *PyTorch ch. 1-4*
2 | Deep Learning Basics <br> *fastbook ch. 4* <br> `01_deep_learning_basics.ipynb`| Deep Learning Basics <br> *PyTorch ch. 5*
3 | *n/a* | Neural Networks <br> *PyTorch ch. 6*
4 | Classification & Regression <br> *fastbook ch. 5 & 6* <br> `02_classification_basics.ipynb` & `03_multilabel_classification_regression.ipynb`| *n/a*
5 | Recommender Systems & Tabular Modeling <br> *fastbook ch. 8 & 9* <br> `04_recommender_systems.ipynb` & `05_tabular_modeling.ipynb`| *n/a*
6 | Computer Vision 1: Image Preprocessing <br> *fastbook ch. 7* <br> `06_image_preprocessing.ipynb`| Computer Vision 1: Images <br> *PyTorch ch. 7*
7 | Computer Vision 2: CNNs <br> *fastbook ch. 13* <br> `07_cnns.ipynb`| Computer Vision 2: CNNs <br> *PyTorch ch. 8*
8 | Computer Vision 3: ResNet <br> *fastbook ch. 14* <br> `08_resnet.ipynb`| Computer Vision 3: CT Scans <br> *PyTorch ch. 9*
9 | NLP 1: Text Preprocessing <br> *fastbook ch. 10* <br> `09_text_preprocessing_classifier.ipynb` | *n/a*
10 | NLP 2: RNNs <br> *fastbook ch. 12* <br> `10_rnns.ipynb` | *n/a*
11 | NLP 3: Transformers <br> `11_transformers.ipynb` and `other_transformer_resources` | *n/a*
12 | Productionization <br> *fastbook ch. 2 & 3* <br> `12_productionization.ipynb` | Deployment <br> *PyTorch ch. 15*
**May 3, 5PM** | **Final Project Due** | 

## Running the Notebooks
Deep learning requires a lot of memory and it is preferred to use GPUs because CPUs are too slow. There are two options for using these notebooks. 

**1. You can upload the files from this repo into Google Drive and open them in Google Colab**
- This will allow you to run all the programs in the Google Cloud
- You get a certain amount of GPU access for free, or can pay $10/month for unlimited
- To swtich to a GPU in Colab, you click *Runtime* --> *Change Runtime Type* --> *Hardware Accelerator* --> *GPU* --> *Save*.
- If you choose this option, you will not need to set up an environment, because the fastbook installation at the top of the script will do all of that for you.

**2. You can download this repo and run it in your own code environment**
- You will need to learn how to switch to GPUs in your own system
- You will also need to connect this code to the fastbook repo and their environment

#### _If you choose to run the notebooks locally, you'll need to set up a code environment:_

A code environment allows you to install and use certain packages and tools without conflicting with other programs / environments you have running. For more details about environments, see <a href="http://www.erdosinstitute.org/programs/asynchronous/software-engineering-for-data-scientists/" target="_blank">Erdős' software enginnering course</a>, created by Kevin Nowland.

To set up your environment for this course, run this line of code in your terminal:
`conda env create -f environment.yml`

When you want to work on these pages, activate the environment, run this code in your terminal:
`conda activate deep-learning`

When you are finished working, deactivate the environment with:
`conda deactivate`

If you are working in VSCode, for each notebook, go to the top right where it sayd *"Select Kernel"*, click *"From Environments"* and then select *"deep-learning"*
