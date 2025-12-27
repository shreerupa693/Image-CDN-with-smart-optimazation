# Image-CDN-with-smart-optimazation
Automatic image compression,smart cropping based on face detection.
func optimizeimage(input [] byte,width int,format string)([]byte,error){
 if format == "webp"{
  return converttoweb(input,80)
 }
 if width > 800{
  return progressiveJPEG(input,width)
 }
return progressiveJPEG(input,width)
 }
 return resizeimage(input,width)
}
 
