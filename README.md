Phishing is a widespread tactic used to trick innocent people into disclosing their personal
information by using bogus websites. Phishing website URLs are designed to steal personal
data, including user names, passwords, and online financial activities. Phishers employ
websites that resemble those genuine websites both aesthetically and linguistically. Utilizing
anti-phishing methods to identify phishing is necessary to stop the rapid advancement of
phishing techniques as a result of advancing technology. A strong tool for thwarting phishing
assaults is machine learning. Attackers frequently use phishing because it is simpler to fool a
victim into clicking a malicious link that looks authentic than to try to get past a computer’s
security measures. The malicious links within the message body are intended to appear to go to
the spoofed company utilizing that company’s logos and other genuine information. In the
method that is being presented, machine learning is used to create a revolutionary approach for
detecting phishing websites. Naive Bayes is the model we utilized in our suggested strategy to
identify phishing websites based on aspects of URL significance. By extracting and comparing
different characteristics between legitimate and phishing URLs, the suggested method uses
Navi Bayes,SVM,Logistic Regression and SGD classifier to identify phishing URLs. The
studies’ findings demonstrate that the suggested approach successfully identifies legitimate
websites from bogus ones in real time.

METHODOLOGY
1.DATASET:
...............
URLs of benign websites were collected from www.alexa.com and The URLs of phishing
websites were collected from www.phishtank.com. The data set consists of total 36,711 URLs
which include 17058 benign URLs and 19653 phishing URLs. Benign URLs are labelled as “0” and phishing URLs are labelled as “1”.


2.FEATURE EXTRACTION:
-------------------------
We have implemented python program to extract features from URL. Below are the features
that we have extracted for detection of phishing URLs

1) Presence of IP address in URL:If IP address present in URL then the feature is set to 1
else set to 0. Most of the benign sites do not use IP address as an URL to download a
webpage. Use of IP address in URL indicates that attacker is trying to steal sensitive
information.
 2) Presence of @ symbol in URL: If @ symbol present in URL then the feature is set to 1
else set to 0. Phishers add special symbol @ in the URL leads the browser to ignore
everything preceding the “@” symbol and the real address often follows the “@” symbol

3) Number of dots in Hostname: Phishing URLs have many dots in URL. For example
http://shop.fun.amazon.phishing.com, in this URL phishing.com is an actual domain name, whereas use of “amazon” word is to trick users to click on it. Average number of dots in
benign URLs is 3. If the number of dots in URLs is more than 3 then the feature is set to 1
else to 0.

4) Length of Host name: Average length of the benign URLs is found to be a 25, If URL’s
length is greater than 25 then the feature is set to 1 else to 0

5) Presence of sensitive words in URL: Phishing sites use sensitive words in its URL so that
users feel that they are dealing with a legitimate webpage. Below are the words that found
in many phishing URLs :- 'confirm', 'account', 'banking', 'secure', 'ebyisapi', 'webscr',
'signin', 'mail', 'install', 'toolbar', 'backup', 'paypal', 'password', 'username', etc;

CONCLUSION:
--------------
The phishing detection mechanism aims to enhance existing blacklist methods and protect users from
malicious login forms. Our research work introduces a new dataset called PILU-90K, which
researchers can utilize to train and evaluate their approaches. This dataset consists of legitimate login
URLs, which are highly representative of real-world phishing detection scenarios. In our study, we
explored various URL-based detection models that employed deep learning and machine learning
solutions. These models were trained using both phishing and legitimate home URLs. One significant
advantage of our approach is its ability to achieve a low false-positive rate when classifying this type
of URL. Among the different models we evaluated, the combination of TFIDF with N-gram and the
LR algorithm yielded the best results, with an accuracy of 96.50%. This outperformed the current
state-of-the-art methods, as discussed in Section II. Our approach offers three main advantages
compared to existing methods: Independence from external services: Unlike descriptive methods that
rely on features such as WHOIS domain age, Google or Alexa page rankings, or online blacklists, our
approach does not depend on external services
