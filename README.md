# AutoSeatCode

This is a test suite written using cucumber-ghenkins-selenium to get a summary of a basic configuration of a Seat Ibiza from https://configurador.seat.es/ .

Requirements:
  - JAVA JDK 1.8 installed, path added to "path" and "JAVA_HOME" environment variable
  - Google Chrome 108.0.5359
  - Chrome WebDriver 108.0.5359.71 placed on C:/BrowserDrivers
  - IntellIj 2022.2.3
    - plugin cucumber for java installed and enabled
    - plugin gherkin installed and enabled
    - plugin IntelliBot @SeleniumLibrary disabled/unistalled.
    - maven extension installed

How to install
  - Download the content of the repository
      - On file ConfiguratorPageSteps, line 66, replace path to downloads for your own path to downloads.
  - On mvn console(from IntelIj):
    - mvn clean
    - mvn install //Dependencies are now installed. Some companies can have problems with their proxies/firewalls at this step.

How to run test:
  - On TestRunner.java execute "public class TestRunner" (green arrow at left of the class), some fails will appear like "step undefined", don't take care about it.
  - On ConfigureIBIZA.feature execute "Scenario:" (green arrow at left). The Test must start.
  
Test Report
  - cucumber report is saved on AutoTest-SeatCode/target/cucumber-report. Use a webbrowser to open it.
