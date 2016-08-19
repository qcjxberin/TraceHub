# TraceHub

TraceHub is to provide centralized logging for Web and service applications through extending System.Diagnostics of .NET Framework. Traces from service applications could be displayed in TraceHub’s logging page.

HubTraceListener is a derived from TraceListenerBase of Essential.Diagnostics, while Essential.Diagnostics is an extension of System.Diagnostics, providing structure tracing and logging. Your .NET applications utilizing System.Diagnostics can utilize TraceHub through HubTraceListner without you altering one line of application codes, since trace listeners could be injected through app.config.

TraceHub Console is a Windows console application that displays traces aggregated in TraceHub which will push traces to the Console when traces arrive. The Console is an alternative to TraceHub’s logging page.

TraceHub is fast and consuming very little system resources in all ends. Being injected with HubTraceListener, a service application sitting in the same zone with TraceHub could write 5000 lines of traces in 0.02 second, and it takes 8 seconds to push the traces from TraceHub to the Console or the logging page. And this could happen when your service applications and TraceHub are located in Oregon, US, while the Console or the Web browser is in Brisbane, Australia.

Currently, the codebase is maintained at https://github.com/zijianhuang/TraceHub , the project management is carried out at https://www.fonlow.com:8443/redmine/projects/tracetoweb/issues . Please feel free to raise issues at the Issues section of Github.

The codebase is almost ready for Beta now...