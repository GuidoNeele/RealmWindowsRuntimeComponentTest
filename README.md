# RealmWindowsRuntimeComponentTest
This repository is made to investigate a build error during a build of a Windows Universal Windows Runtime Component which includes Realm. Related Stack Overflow question: https://stackoverflow.com/questions/49449263/universal-windows-10-16299-windows-runtime-component-build-error

Just download repository and build project and build error will appear in output.

# Build error
When building project the following error is displayed

```
ExportWindowsMDFile:
  C:\Program Files (x86)\Microsoft Visual Studio\2017\Community\MSBuild\Microsoft\VisualStudio\v15.0\AppxPackage\winmdexp.exe /mp:obj\x86\Debug\RealmTest.UWP.BackgroundSync.compile.pdb
  /pdb:obj\x86\Debug\RealmTest.UWP.BackgroundSync.pdb
  /out:obj\x86\Debug\RealmTest.UWP.BackgroundSync.winmd
  /utf8output
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\Microsoft.CSharp.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\Microsoft.VisualBasic.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\Microsoft.Win32.Primitives.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\mscorlib.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\netstandard.dll
  /reference:C:\Users\guido\.nuget\packages\newtonsoft.json\11.0.1\lib\netstandard2.0\Newtonsoft.Json.dll
  /reference:C:\Users\guido\.nuget\packages\realm.databinding\1.2.0\lib\netstandard1.0\Realm.DataBinding.dll
  /reference:C:\Users\guido\.nuget\packages\realm.database\2.2.0\lib\netstandard1.4\Realm.dll
  /reference:C:\Users\guido\.nuget\packages\realm\2.2.0\lib\netstandard1.4\Realm.Sync.dll
  /reference:C:\Users\guido\.nuget\packages\remotion.linq\2.1.2\lib\portable-net45+win+wpa81+wp80\Remotion.Linq.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.AppContext.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Buffers.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Collections.Concurrent.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Collections.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Collections.Immutable.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Collections.NonGeneric.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Collections.Specialized.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.ComponentModel.Annotations.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.ComponentModel.Composition.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.ComponentModel.DataAnnotations.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.ComponentModel.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.ComponentModel.EventBasedAsync.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.ComponentModel.Primitives.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.ComponentModel.TypeConverter.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Configuration.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Console.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Core.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Data.Common.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Data.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Data.SqlClient.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Diagnostics.Contracts.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Diagnostics.Debug.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Diagnostics.FileVersionInfo.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Diagnostics.Process.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Diagnostics.StackTrace.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Diagnostics.TextWriterTraceListener.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Diagnostics.Tools.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Diagnostics.TraceSource.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Diagnostics.Tracing.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Drawing.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Drawing.Primitives.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Dynamic.Runtime.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Globalization.Calendars.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Globalization.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Globalization.Extensions.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.IO.Compression.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.IO.Compression.FileSystem.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.IO.Compression.ZipFile.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.IO.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.IO.FileSystem.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.IO.FileSystem.DriveInfo.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.IO.FileSystem.Primitives.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.IO.FileSystem.Watcher.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.IO.IsolatedStorage.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.IO.MemoryMappedFiles.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.IO.Pipes.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.IO.Ports.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.IO.UnmanagedMemoryStream.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Linq.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Linq.Expressions.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Linq.Parallel.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Linq.Queryable.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Net.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Net.Http.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Net.Http.Rtc.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Net.HttpListener.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Net.Mail.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Net.NameResolution.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Net.NetworkInformation.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Net.Ping.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Net.Primitives.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Net.Requests.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Net.Security.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Net.ServicePoint.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Net.Sockets.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Net.WebClient.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Net.WebHeaderCollection.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Net.WebProxy.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Net.WebSockets.Client.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Net.WebSockets.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Numerics.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Numerics.Vectors.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Numerics.Vectors.WindowsRuntime.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.ObjectModel.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Reflection.Context.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Reflection.DispatchProxy.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Reflection.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Reflection.Extensions.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Reflection.Metadata.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Reflection.Primitives.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Reflection.TypeExtensions.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Resources.Reader.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Resources.ResourceManager.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Resources.Writer.dll
  /reference:C:\Users\guido\.nuget\packages\system.runtime.compilerservices.unsafe\4.4.0\ref\netstandard2.0\System.Runtime.CompilerServices.Unsafe.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Runtime.CompilerServices.VisualC.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Runtime.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Runtime.Extensions.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Runtime.Handles.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Runtime.InteropServices.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Runtime.InteropServices.RuntimeInformation.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Runtime.InteropServices.WindowsRuntime.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Runtime.Numerics.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Runtime.Serialization.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Runtime.Serialization.Formatters.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Runtime.Serialization.Json.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Runtime.Serialization.Primitives.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Runtime.Serialization.Xml.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Runtime.WindowsRuntime.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Runtime.WindowsRuntime.UI.Xaml.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Security.AccessControl.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Security.Claims.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Security.Cryptography.Algorithms.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Security.Cryptography.Cng.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Security.Cryptography.Csp.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Security.Cryptography.Encoding.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Security.Cryptography.Primitives.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Security.Cryptography.X509Certificates.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Security.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Security.Principal.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Security.Principal.Windows.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Security.SecureString.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.ServiceModel.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.ServiceModel.Duplex.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.ServiceModel.Http.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.ServiceModel.NetTcp.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.ServiceModel.Primitives.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.ServiceModel.Security.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.ServiceModel.Web.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.ServiceProcess.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Text.Encoding.CodePages.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Text.Encoding.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Text.Encoding.Extensions.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Text.RegularExpressions.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Threading.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Threading.Overlapped.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Threading.Tasks.Dataflow.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Threading.Tasks.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Threading.Tasks.Parallel.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Threading.Thread.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Threading.ThreadPool.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Threading.Timer.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Transactions.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Transactions.Local.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.ValueTuple.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Web.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Web.HttpUtility.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Windows.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Xml.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Xml.Linq.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Xml.ReaderWriter.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Xml.Serialization.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Xml.XDocument.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Xml.XmlDocument.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Xml.XmlSerializer.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Xml.XPath.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\System.Xml.XPath.XDocument.dll
  /reference:<nuget path>\microsoft.netcore.universalwindowsplatform\6.0.8\ref\uap10.0.15138\WindowsBase.dll
  /reference:<Windows Kits Path>\10\References\10.0.16299.0\Windows.ApplicationModel.Calls.CallsVoipContract\2.0.0.0\Windows.ApplicationModel.Calls.CallsVoipContract.winmd
  /reference:<Windows Kits Path>\10\References\10.0.16299.0\Windows.ApplicationModel.SocialInfo.SocialInfoContract\2.0.0.0\Windows.ApplicationModel.SocialInfo.SocialInfoContract.winmd
  /reference:<Windows Kits Path>\10\References\10.0.16299.0\Windows.ApplicationModel.StartupTaskContract\2.0.0.0\Windows.ApplicationModel.StartupTaskContract.winmd
  /reference:<Windows Kits Path>\10\References\10.0.16299.0\Windows.Devices.Custom.CustomDeviceContract\1.0.0.0\Windows.Devices.Custom.CustomDeviceContract.winmd
  /reference:<Windows Kits Path>\10\References\10.0.16299.0\Windows.Devices.DevicesLowLevelContract\3.0.0.0\Windows.Devices.DevicesLowLevelContract.winmd
  /reference:<Windows Kits Path>\10\References\10.0.16299.0\Windows.Devices.Printers.PrintersContract\1.0.0.0\Windows.Devices.Printers.PrintersContract.winmd
  /reference:<Windows Kits Path>\10\References\10.0.16299.0\Windows.Devices.SmartCards.SmartCardBackgroundTriggerContract\3.0.0.0\Windows.Devices.SmartCards.SmartCardBackgroundTriggerContract.winmd
  /reference:<Windows Kits Path>\10\References\10.0.16299.0\Windows.Devices.SmartCards.SmartCardEmulatorContract\5.0.0.0\Windows.Devices.SmartCards.SmartCardEmulatorContract.winmd
  /reference:<Windows Kits Path>\10\References\10.0.16299.0\Windows.Foundation.FoundationContract\3.0.0.0\Windows.Foundation.FoundationContract.winmd
  /reference:<Windows Kits Path>\10\References\10.0.16299.0\Windows.Foundation.UniversalApiContract\5.0.0.0\Windows.Foundation.UniversalApiContract.winmd
  /reference:<Windows Kits Path>\10\References\10.0.16299.0\Windows.Gaming.XboxLive.StorageApiContract\1.0.0.0\Windows.Gaming.XboxLive.StorageApiContract.winmd
  /reference:<Windows Kits Path>\10\References\10.0.16299.0\Windows.Graphics.Printing3D.Printing3DContract\4.0.0.0\Windows.Graphics.Printing3D.Printing3DContract.winmd
  /reference:<Windows Kits Path>\10\References\10.0.16299.0\Windows.Networking.Connectivity.WwanContract\1.0.0.0\Windows.Networking.Connectivity.WwanContract.winmd
  /reference:<Windows Kits Path>\10\References\10.0.16299.0\Windows.Services.Store.StoreContract\2.0.0.0\Windows.Services.Store.StoreContract.winmd
  /reference:<Windows Kits Path>\10\References\10.0.16299.0\Windows.Services.TargetedContent.TargetedContentContract\1.0.0.0\Windows.Services.TargetedContent.TargetedContentContract.winmd
  /reference:<Windows Kits Path>\10\References\10.0.16299.0\Windows.System.Profile.ProfileHardwareTokenContract\1.0.0.0\Windows.System.Profile.ProfileHardwareTokenContract.winmd
  /reference:<Windows Kits Path>\10\References\10.0.16299.0\Windows.System.Profile.ProfileSharedModeContract\2.0.0.0\Windows.System.Profile.ProfileSharedModeContract.winmd
  /reference:<Windows Kits Path>\10\References\10.0.16299.0\Windows.UI.ViewManagement.ViewManagementViewScalingContract\1.0.0.0\Windows.UI.ViewManagement.ViewManagementViewScalingContract.winmd
  /reference:<Windows Kits Path>\10\UnionMetadata\facade\Windows.winmd
  obj\x86\Debug\RealmTest.UWP.BackgroundSync.winmdobj
WINMDEXP : error WME1007: Could not resolve reference 'Assembly(Name=System.Collections, Version=4.2.1.0, Culture=neutral, PublicKeyToken=b03f5f7f11d50a3a)'.

Build FAILED.


"C:\DEV\Test\Realm\RealmTest\RealmTest.UWP.BackgroundSync\RealmTest.UWP.BackgroundSync.csproj" (default target) (1) ->
(ExportWindowsMDFile target) -> 
  WINMDEXP : error WME1007: Could not resolve reference 'Assembly(Name=System.Collections, Version=4.2.1.0, Culture=neutral, PublicKeyToken=b03f5f7f11d50a3a)'.

    1 Warning(s)
    1 Error(s)

Time Elapsed 00:00:01.22
========== Build: 0 succeeded, 1 failed, 0 up-to-date, 0 skipped ==========
```
