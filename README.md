# Raise_the_terrain
<div class="panel-body">
    <span id="user_id" data-id="222"></span>

    

    <!-- Progress vs Score -->

    <!-- Task Body -->
    <h3>Isometric projection</h3>

<p>The following image is the isometric projection of a grid:</p>

<p><img src="https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/9/10a0e33273cfd07850f6d91ead6bce73dfc6b32b.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOU65GPZGY3%2F20210516%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210516T015123Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=89c9be4ffc0e9678d93004586f568d846a2e19936039a568cd0d189e97601174" alt="" style=""></p>

<p>Given the following altitudes,</p>

<pre><code>120 60 40 60 20 -20 -80 -120
40 20 30 30 -10 -40 -90 -110
20 30 10 06 -6 -20 -26 -90
00 -6 10 10 -6 -20 -20 -40
-20 -20 -18 -14 -40 -20 -20 -30
-10 -10 -10 -10 -8 -20 -20 -30
20 10 10 10 10 04 10 -10
30 24 24 22 20 18 14 16
</code></pre>

<p>the grid should look like this:</p>

<p><img src="https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/9/a7111e7e11bd23c0b66e79f97f32d879e89dcff5.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOU65GPZGY3%2F20210516%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210516T015123Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=f36957b9cc1eb562a1364d462c18a7c128332dfc17db0c68baea6e214cd0243c" alt="" style=""></p>

<h3>Maths</h3>

<p>To draw a grid using isometric projection, you’ll need to convert 3D coordinates (coordinates in the real world) to 2D coordinates (coordinates on the screen), as follows:</p>

<p><img src="https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/9/e07c3b1a34523b467eec5235b646194617354b42.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIARDDGGGOU65GPZGY3%2F20210516%2Fus-east-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20210516T015123Z&amp;X-Amz-Expires=86400&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=de7bc8e2e0b3d2090c522d11cef979deda58d8c1362587bc043b33f3ff7b94dd" alt="" style=""></p>

<p>You can choose to incline your grid as much as you want.</p>

<pre><code>WX = inclination * X - inclination * Y;
WY = (1 - inclination) * X + (1 - inclination) * Y - Z;
</code></pre>

<p>where an <code>inclination</code> of 70% would have a value of <code>0.7</code> in this above equation.</p>

<h3>Requirements</h3>

<ul>
<li>Usage: <code>terrain file</code></li>
<li>Draw a grid using an isometric projection</li>
<li>The grid must be described in a file (see above example)</li>
<li>The color used to draw the grid doesn’t matter (same for the background)</li>
<li>The grid doesn’t need to be <em>exactly</em> the same as the one shown above. But make sure you have a coherent isometric projection.</li>
<li>Your grid must be centered and takes as much space as possible on the screen. We should be able to see the whole screen.</li>
<li>Your program should end when the user is pressing the <code>ESC</code> key</li>
</ul>

  </div>
