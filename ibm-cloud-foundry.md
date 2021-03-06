## Overview 
These are the steps I followed with help from #st_canada scholars @NikitaBaranov @Danilo.Britto.Scholar

## Contributors: 
Chromilo

1. Create an IBM Cloud account https://cloud.ibm.com/ for yourself.
2. Login to the dashboard and create and public Cloud Foundry environment https://cloud.ibm.com/cloudfoundry/public. Name the application python-helloworld-chromilo.
3. After the CF sample app is created, a guideline appears asking you to install the prerequisites like IBM Cloud CLI and creating some config files.
4. Clone the python-helloworld exercise repo.
5. Create a manifest.yaml file in your python-helloworld folder with the following text copied from the IBM Cloud Foundry instructions screen. Change the 'name' to be python-helloworld-chromilo.

  applications:
  - name: pytone-helloworld-chromilo
    random-route: true
    memory: 128M
    
6. Create startup file "Procfile" with one line text "web: python app.py" in the save python-helloworld folder.
7. Edit the app.py code to listen on port 8080 or some other port because the default listening port for flask is 5000. If you don't do this, the readiness probe fails.

if __name__ == "__main__":
    ## stream logs to app.log file
    logging.basicConfig(filename='app.log',level=logging.DEBUG)
    app.run(host='0.0.0.0',port='8080')
    
8. Download IBM Cloud CLI https://www.ibm.com/cloud/cli, install and reboot your computer.
9. Launch Powershell CLI in admin-mode.
10. Login to IBM Cloud by typing "ic login". Enter your email and password to login.
11. Change folder path to cloned repo containing python-helloworld exercise.
12. Push the changes to your IBM Cloud Foundry deployed application "ibmcloud cf push".
13. After a cf push, you can check the logs via "ibmcloud cf log" or from the IBM Cloud dashboard.
14. Launch https://python-helloworld-chromilo-quiet-oribi-kw.mybluemix.net/
