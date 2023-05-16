# Deep_Learning
Our code uses two convolutional neural network architectures, DenseNet-121 and a baseline CNN, for image classification. DenseNet-121 is efficient at learning feature representations with fewer parameters. The baseline CNN is likely for comparison.
To start with the project,
First go to the physionet website and download the dataset https://physionet.org/content/apnea-ecg/
The dataset consist of the following: The data consist of 70 records, divided into a learning set of 35 records (a01 through a20, b01 through b05, and c01 through c10), and a test set of 35 records (x01 through x35), all of which may be downloaded from this page. Recordings vary in length from slightly less than 7 hours to nearly 10 hours each. Each recording includes a continuous digitized ECG signal, a set of apnea annotations (derived by human experts on the basis of simultaneously recorded respiration and related signals), and a set of machine-generated QRS annotations (in which all beats regardless of type have been labeled normal). In addition, eight recordings (a01 through a04, b01, and c01 through c03) are accompanied by four additional signals (Resp C and Resp A, chest and abdominal respiratory effort signals obtained using inductance plethysmography; Resp N, oronasal airflow measured using nasal thermistors; and SpO2, oxygen saturation).
Now, copy the downloaded zip file and upload it to google drive account
Mount your google drive account with the google colab using the following code : from google.colab import drive
drive.mount('/content/drive', force_remount=True)
Now using the code :- import zipfile

zip_ref = zipfile.ZipFile(path, 'r')
zip_ref.extractall('/content/my_data_folder')
zip_ref.close()
Extract all the files and save it to your specified path inside google colab
Note- The google colab account loses its access with the colabaoratory , when the runtime gets disconnected.
