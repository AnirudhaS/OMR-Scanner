The XML template stores the coordinate information of the sheet, so as to check after post processing whether any blobs existsin the area.
There is an XML file 'first_template.xml' which is relevant to the uploaded PDF. It is self explanatory.
The sheet processing is done in the namespace 'XMLRead' under the file Sheet.cs

The template can be modified to adapt to different sheets. But some trial-error should be done to verify the image processing results as if the blobs are proper or not.
