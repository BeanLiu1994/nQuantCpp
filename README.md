# nQuantCpp
nQuantCpp includes top 6 color quantization algorithms for visual c++ producing high quality optimized images.

Divisive hierarchical clustering algorithm,
Fast pairwise nearest neighbor based algorithm, 
NeuQuant Neural-Net Quantization Algorithm, 
Xialoin Wu's fast optimal color quantizer, 
Efficient, Edge-Aware, Combined Color Quantization and Dithering,
Spatial color quantization

Fast pairwise nearest neighbor based algorithm minimized color loss for photo having red lips and supports 256 or less colors with transparency. NeuQuant Neural-Net Quantization Algorithm produces smooth photo quantization especially for natual landscape photo and fully supports image having transparent color. Xialoin Wu's fast optimal color quantizer fully supports image having transparent color. DL3 Quantization supports 256 or less colors. Spatial color quantization supports 64 or less colors. nQuantCpp also provides a command line wrapper in case you want to use it from the command line.

Either download nQuantCpp from this site or add it to your Visual Studio project seamlessly.
The main features show up to discuss would be the error diffusion and dithering.

Here some examples of output:

Original image<img src="https://i.stack.imgur.com/fOcIL.png" /><br>
Reduced to 256 colors by Xialoin Wu's fast optimal color Quantization Algorithm<img src="https://i.stack.imgur.com/PGWVF.png" /><br>
Reduced to 256 colors by NeuQuant Neural-Net Quantization Algorithm<img src="https://i.stack.imgur.com/4jLkg.png" /><br>
Reduced to 256 colors by Fast pairwise nearest neighbor based algorithm<img src="https://i.stack.imgur.com/RX2dK.png" /><br><br>
Original photo<img src="https://i.stack.imgur.com/jFvEG.jpg" /><br>
Reduced to 256 colors by NeuQuant Neural-Net Quantization Algorithm<img src="https://i.stack.imgur.com/yJIjQ.gif" />
Reduced to 256 colors by Fast pairwise nearest neighbor based algorithm<img src="https://i.stack.imgur.com/dPTml.gif" />

<p>Original image<br><img src="https://i.stack.imgur.com/9jL4F.jpg" /><br>
<b><a href="http://www.cs.joensuu.fi/sipu/pub/Threshold-JEI.pdf">Fast pairwise nearest neighbor based algorithm with CIELAB color space</a></b> with 16 colors<br>
High quality and fast<br>
<img src="https://i.stack.imgur.com/8kVq1.png" alt="Fast pairwise nearest neighbor based algorithm with CIELAB color space with 16 colors"></p>
<p><b><a href="http://cg.cs.tsinghua.edu.cn/people/~huanghz/publications/TIP-2015-CombinedColorQuantization.pdf">Efficient, Edge-Aware, Combined Color Quantization and Dithering</a></b> with 16 colors<br>
Higher quality for 32 or less colors but slower<br>
<img src="https://i.stack.imgur.com/WHpXY.png" alt="Efficient, Edge-Aware, Combined Color Quantization and Dithering with 16 colors"></p>
<p><b><a href="https://people.eecs.berkeley.edu/~dcoetzee/downloads/scolorq/">Spatial color quantization</a></b> with 16 colors<br>
Higher quality for 32 or less colors but the slowest<br>
<img src="https://i.stack.imgur.com/lVoHK.png" alt="Spatial color quantization with 16 colors"></p>

If you are using the command line. Assuming you are in the same directory as nQuantCpp.exe, you would enter: nQuantCpp yourImage.jpg /m 16

nQuantCpp will quantize yourImage.jpg and create yourImage-PNNLABquant16.png in the same directory.

The readers can see coding of the error diffusion and dithering are quite similar among the above quantization algorithms. 
Each algorithm has its own advantages. I share the source of color quantization to invite further discussion and improvements.
Such source code are written in C++ to gain best performance. It is readable and convertible to c#, java, or javascript.
Welcome for C++ experts for further improvement or provide color quantization algorithms better than the above algorithms.
Please send email to miller.chan@gmail.com to report issues or give suggestions.
