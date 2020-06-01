# first_repository
Online examination video surveillance system
Here we are considering 3 anomalies
1.impersonation(some else writing exam on one's behalf)
2.gadget usage(I considered book; you can consider any object among 80 objects detected by ImageAI)
3.Brightness, contrast effect





CapturingAndStoring:
Here we capture video, extract frames from them and store them
Brightness module:
Here we check for brightness of frames and modify if it is less than 128 units, also we perform auto contrast change
Object detection module:
In this module we detect if book is present, if so i will return 1 ; if more than one person is present in the image then i would return 2
else 0
Test anomaly detection:
Here i will check if image has atleast 1 person if not if not i would increment anomaly count, else i would check for multiple person if so 
then i would increment anomaly count, then i would check for existance of any object, here i considered anomaly object to be book, we can 
even add cell phone etc etc( abount 80 objects are detected by imageAI) to it.
Then I calculated probabilty of occurance of anomaly and if it is more than threshold(your choice , i considered it to be 0.441) then say that 
there is some anomaly else no anomaly.
