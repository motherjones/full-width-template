# Header [need to explain this]


# Basic Hed, Dek, Paragraphs
Use this `<section>` type for a basic section with a hed, dek, and paragraphs:

	<section>
		<h2>The hed goes here</h2>
		<p class="subhead">The dek goes here.</p>
		<p><strong>Bold first words:</strong> Here is where a paragraph will go. In this
		 example, the first few words are bolded, but you can delete the "<strong>" tags 
		 if you don't want this effect.</p>
	</section>

This section will look like this:

INSERT SCREENSHOT

As you can see, the hed of each section gets wrapped in `<h2>` tags, which are styled in the CSS to be larger and have a small icon image to the left (here it appears as a tiny oil tower). To change the icon image to better fit your story, find where it says `#shell960 h2` in the CSS, and replace the url within `background-image: url('TKTKTKTKTKURL')` with the url of the image you want to use.

All of your deks will go in `<p>` tags with the class ` "subhead" `. 

Paragraphs are wrapped with opening and closing `<p>` tags. You can add as many paragraphs as you like to a section.


# 630px Images


Use this type of `<section>` if you have an image that you would like to be displayed in-line at 630 px. 

	<section>
		<h2>the hed goes here</h2>
		<p class="subhead">The dek goes here.</p>
		<p>Here is a sample paragraph.</p>
		<p>If your section is just going to include an image and no paragraphs, just delete these.</p>
		<figure>
			<img alt="" class="width630" src="http://assets.motherjones.com/politics/2014/04/federal-lobbying-political-giving.png" />
		</figure>	
	</section>
	
This looks like this:

ADD SCREENSHOT

First, replace the dummy hed, dek, and paragraphs with your content, as explained above. Next you will replace the image url in the `<figure>` tag (in the quotation marks after src=) with a link to your image.

Usually, you want your image to stay in-line with the rest of the story at 630 px. If this is your plan, crop your image to 630 px wide before uploading. Talk to the Interactive team before uploading your images, because they have a preferred method for uploading and storing the images. However, if you need to do it yourself, there is an alternative way of adding images. In the Drupal edit view, expand the **File Attachments** section and attach your cropped image. 

ADD SCREENSHOT OF WHERE TO ADD IMAGE
When it uploads, you will be provided with a url. You can then paste this url into the HTML `<figure>` tag (in the quotation marks after `src=`).


# Images with Captions

Use this HTML if your section is going to have a hed, image, and caption.

	    <section>
		<h2>Hed</h2>
		<figure>
        	<img alt="" class="width630" src="https://www.motherjones.com/files/taylor-dean-giant630.jpg" />
			<figcaption>Here is where the photo caption goes.</figcaption>
        </figure>
	</section>
	
Which looks like this:

SCREENSHOT

Like the example above, this image will desplay inline at 630px, and should be cropped to 630 before uploading. Captions go in `<figcaption>` tags, which are nested inside the `<figure>` tag.


# Large, standalone Images

This is a large standalone image. [EXPLANATION TK]


# 850px Images

Use this type of `<section>` when you want an image to be 850px wide, so that it extends beyond the rest of the story. 

	<section>
		<figure>
			<img alt="" class="width850" src="http://assets.motherjones.com/media/2014/05/chast-jan-1985-850.jpg" />
			<figcaption>Here is the caption for the image.</figcaption>
		</figure>
	</section>

This is achieved by giving the `<img>` class ` "width850" ` instead of the standard ` "width630" `. (Example: [These cartoons](http://www.motherjones.com/media/2014/05/roz-chast-mother-jones-cartoons) are all displayed at 850 px wide.) 

If you are using this type of section for an image, you should crop the image to 850px width before uploading.

# Bulleted Lists

Use this type of section if you want to include a bulleted list. 

    <section>
			<h2>The Hed Goes Here</h2>
			<p class="subhead">The Dek goes here.</p>
			<nav>
				<ul>
					<li>This is a list item.</li>
					<li>This is another list item.</li>
					<li>And here is a third.</li>
           	 	</ul>
			</nav>
	</section>
 
Which will display like this:

SCREENSHOT

