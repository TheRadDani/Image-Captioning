# Image-Captioning

<p>This repository contains the code and models for image captioning using the COCO 2017 dataset.</p>

<h2>Requirements</h2>

<p>You can find the project dependencies in <a href="requirements.txt">requirements.txt</a>.</p>


<p>To download the COCO 2017 dataset, please follow the instructions on the <a href="https://cocodataset.org/#download">official website</a>.</p>

<h2>Usage</h2>

<p>To train a model, first, download the dataset and preprocess the images and captions using the <code>preprocess.py</code> script. The script can be run as follows:</p>

<pre><code>python preprocess.py --data-root /path/to/coco2017 --output /path/to/output</code></pre>

<p>This will create an HDF5 file containing the preprocessed images and captions.</p>

<p>Next, run the <code>train.py</code> script to train the model:</p>

<pre><code>python train.py --input /path/to/preprocessed/data.hdf5 --output /path/to/output</code></pre>

<p>To generate captions for new images using a trained model, run the <code>generate.py</code> script:</p>

<pre><code>python generate.py --model /path/to/trained/model.pth --image /path/to/image.jpg</code></pre>

<h2>References</h2>

<ul>
  <li>COCO 2017 dataset: <a href="https://cocodataset.org/#download">https://cocodataset.org/#download</a></li>
</ul>

<h2>License</h2>

<p>This project is licensed under the MIT License. See the <a href="LICENSE">LICENSE</a> file for details.</p>
