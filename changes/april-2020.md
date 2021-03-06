# Changelog  / Apr 2020

## UI

We have done some interesting changes to the UI in order to provide better user experience and usability for our solution.

### Progress

We have changed the way progress is tracked from being shown only in percentage (%) to be shown as entries done out of the total entries discovered for the running scan.

![image](https://user-images.githubusercontent.com/1631073/78462400-3e655d80-76da-11ea-8d0b-a8c954b539cb.png)

### Scan Configuration

We have added a section to view the configurations the scan was started with, this is helpful for copying and verifying scan configuration.

![image](https://user-images.githubusercontent.com/1631073/78462450-ba5fa580-76da-11ea-9f81-68416affa0ec.png)

While the "Runtime Parameters" show the standard screen for live information

![image](https://user-images.githubusercontent.com/1631073/78462459-e3803600-76da-11ea-8761-6dc01b43d147.png)

### Findings Research and Customization

We have greatly enhanced the "run script" option with a powerful editing tool available for every finding, it will replace the "run script" play button with an edit icon

![image](https://user-images.githubusercontent.com/1631073/78462481-162a2e80-76db-11ea-9023-f6ea1e1f7cc3.png)

When clicked a new fully editable window will open that will show the request and will allow you to edit and either "Save as a new issue" or "execute" to run the request again.

![image](https://user-images.githubusercontent.com/1631073/78462529-b5e7bc80-76db-11ea-9690-f75afa254e3e.png)

### PDF and Reporting

We improved the PDF generation functionality to add both the ability to select specific sections of the PDF you might want to generate, and also a new progress bar to show the PDF generation stages and remove the "waiting for unkown time" feeling.

* Custom option

![image](https://user-images.githubusercontent.com/1631073/78462594-5a69fe80-76dc-11ea-9f80-c2c9c2363a7f.png)

* Section selection

![image](https://user-images.githubusercontent.com/1631073/78462607-74a3dc80-76dc-11ea-9fbc-3c9ba4bf6148.png)

* Progress

![image](https://user-images.githubusercontent.com/1631073/78462648-acab1f80-76dc-11ea-8748-df2a746a257c.png)

## Engine

We always prioritize optimizations and scan speed improvements as part of our on going development effort, and we are proud to say that this release have indeed improved our performance in more then 50%!.

If you look at the following comparison done via our Analysis tab, you can see some of the examples to the hard work we did

![image](https://user-images.githubusercontent.com/1631073/78552555-62c35600-7810-11ea-8e92-86635328e4d0.png)

Most noticeable are the time difference (we managed to cut more then 2 hours of scan time), more findings, and more entries.
This change is now part of our production environment and is accessible to all of our users.

## Bug Fixes

* Fix notorious "math bug" where XSS will show non 100% status while scan goes to "Done" status.
* SSRF speed optimizations, greatly increasing scan speed when testing for SSRF.
