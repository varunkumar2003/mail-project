# PYTHON-PROJECT.
import smtplib as s

ob=s.SMTP('smtp.gmail.com',587)
ob.ehlo()
ob.starttls()
ob.login('varunkumar.008@gmail.com','ovlsghkwcriwefpr')
subject="i am single"
body="i need a girlfriend"
massage="subject:{}\n\n{}".format(subject,body)
listall=['gvarunkumar.008@gmail.com','varshith.neeredu@gmail.com']
ob.sendmail('varunkumar.008@gmail.com',listall,massage)
print("sendmail")
ob.quit()
