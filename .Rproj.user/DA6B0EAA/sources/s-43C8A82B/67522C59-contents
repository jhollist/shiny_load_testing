# from R
# This will fire up a browser with the app in it.  Interact with the app as you
# think a user would.  This gets recorded and is re-run for each of the workers
# in the shinycannon step.
# url <- 'https://simpleepashiny.app.cloud.gov/'
url <- "https://cyan.app.cloud.gov/"
#url <- "http://edap-rshiny.rtpnc.epa.gov:3838/cyanuric/"

shinyloadtest::record_session(url)

# from command line
#java -jar shinycannon-1.0.0-b267bad.jar recording.log 'http://edap-rshiny.rtpnc.epa.gov:3838/cyanuric/' --workers 10 --loaded-duration-minutes 5 --output-dir cyan_run4_edap

# from R
df <- shinyloadtest::load_runs("10 workers - 5 minutes - 4GB - 1 Instance" = "./cyan_run5")
shinyloadtest::shinyloadtest_report(df, "cyan_run5.html")

df <- shinyloadtest::load_runs("10 workers - 5 minutes - 2GB - 2 Instance" = "./cyan_run6")
shinyloadtest::shinyloadtest_report(df, "cyan_run6.html")

df <- shinyloadtest::load_runs("10 workers - 5 minutes - 768MB - 3 Instance" = "./cyan_run7")
shinyloadtest::shinyloadtest_report(df, "cyan_run7.html")

df <- shinyloadtest::load_runs("20 workers - 5 minutes - 768MB - 3 Instance" = "./cyan_run8")
shinyloadtest::shinyloadtest_report(df, "cyan_run8.html")
