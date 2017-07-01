# Keyboard-Maestro-Macros
Various Macros I've written for Mac OS [Keyboard Maestro](https://www.keyboardmaestro.com/main/) application.

## Macro Descriptions
1. Transcoding Status.kmmacros
	Every 5 minutes this macro checks if there is a HandbrakeCLI process is running. Once it finds it running it continues checking every 5 minutes for it to stop. Once the process ends it sends a notification to the Pushover Service.
	Requires the Check Unix Process subroutine and the [Pushover Plug-in](https://github.com/kvanh/Keyboard-Maestro-Pushover-Notifications)

## Subroutines

1. Check Unix Process.kmmacros
	Allows Keyboard Maestro to check if a process is running. This can catch Unix processes that the If Application is running statements can't. Returns a text string "true" or "false" if the process is running. Set the process name in variable CheckProcess.
