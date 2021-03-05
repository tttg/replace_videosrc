# replace_videosrc  
In order to scale video in imxv4l2videosrc,we should modifyed crop-meta-width and crop-meta-height.  
But as properities of imxv4l2videosrc,modifyed crop-meta-width and crop-meta-height could not work.  
So we should replace imxv4l2videosrc with different properities of crop-meta-xxx.   
imxv4l2videosrc ==> imxv4l2videosrc crop-meta-width=xx crop-meta-height=xx.  
---------------------------------------------------------------------------------------------------  
gst_element_set_state(data->src, GST_STATE_PAUSED);  
remove_element_src(data);  
create_element_src(data);  
gst_element_set_state(data->src, GST_STATE_PLAYING);  
[QQ:420788046]  
[Email:luwei860123@163.com]  
