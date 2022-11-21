# jenkins workspece error

```

The recommended git tool is: git
using credential github-auth
Cloning the remote Git repository
Cloning with configured refspecs honoured and without tags
Cloning repository git@github.com:tcuts/hc-services.git
ERROR: Failed to clean the workspace
jenkins.util.io.CompositeIOException: Unable to delete '/var/lib/jenkins/workspace/ne-services_RetailUserOTPFeature'. Tried 3 times (of a maximum of 3) waiting 0.1 sec between attempts.
	at jenkins.util.io.PathRemover.forceRemoveDirectoryContents(PathRemover.java:87)
	at hudson.Util.deleteContentsRecursive(Util.java:286)
	at hudson.Util.deleteContentsRecursive(Util.java:275)
	at org.jenkinsci.plugins.gitclient.CliGitAPIImpl$2.execute(CliGitAPIImpl.java:788)
	at hudson.plugins.git.GitSCM.retrieveChanges(GitSCM.java:1226)
	at hudson.plugins.git.GitSCM.checkout(GitSCM.java:1308)
	at org.jenkinsci.plugins.workflow.steps.scm.SCMStep.checkout(SCMStep.java:129)
	at org.jenkinsci.plugins.workflow.steps.scm.SCMStep$StepExecutionImpl.run(SCMStep.java:97)
	at org.jenkinsci.plugins.workflow.steps.scm.SCMStep$StepExecutionImpl.run(SCMStep.java:84)
	at org.jenkinsci.plugins.workflow.steps.SynchronousNonBlockingStepExecution.lambda$start$0(SynchronousNonBlockingStepExecution.java:47)
	at java.base/java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:515)
	at java.base/java.util.concurrent.FutureTask.run(FutureTask.java:264)
	at java.base/java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1128)
	at java.base/java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:628)
	at java.base/java.lang.Thread.run(Thread.java:829)
	Suppressed: java.nio.file.FileSystemException: /var/lib/jenkins/workspace/ne-services_RetailUserOTPFeature/jenkins/results/jenkins.xml: Operation not permitted
		at java.base/sun.nio.fs.UnixException.translateToIOException(UnixException.java:100)
		at java.base/sun.nio.fs.UnixException.rethrowAsIOException(UnixException.java:111)
		at java.base/sun.nio.fs.UnixException.rethrowAsIOException(UnixException.java:116)
		at java.base/sun.nio.fs.UnixFileAttributeViews$Posix.setMode(UnixFileAttributeViews.java:254)
		at java.base/sun.nio.fs.UnixFileAttributeViews$Posix.setPermissions(UnixFileAttributeViews.java:276)
		at java.base/java.nio.file.Files.setPosixFilePermissions(Files.java:2080)
		at jenkins.util.io.PathRemover.makeWritable(PathRemover.java:285)
		at jenkins.util.io.PathRemover.makeRemovable(PathRemover.java:258)
		at jenkins.util.io.PathRemover.removeOrMakeRemovableThenRemove(PathRemover.java:238)
		at jenkins.util.io.PathRemover.tryRemoveFile(PathRemover.java:202)
		at jenkins.util.io.PathRemover.tryRemoveRecursive(PathRemover.java:213)
		at jenkins.util.io.PathRemover.tryRemoveDirectoryContents(PathRemover.java:224)
		at jenkins.util.io.PathRemover.tryRemoveRecursive(PathRemover.java:212)
		at jenkins.util.io.PathRemover.tryRemoveDirectoryContents(PathRemover.java:224)
		at jenkins.util.io.PathRemover.tryRemoveRecursive(PathRemover.java:212)
		at jenkins.util.io.PathRemover.tryRemoveDirectoryContents(PathRemover.java:224)
		at jenkins.util.io.PathRemover.forceRemoveDirectoryContents(PathRemover.java:84)
		... 14 more
	Suppressed: java.nio.file.FileSystemException: /var/lib/jenkins/workspace/ne-services_RetailUserOTPFeature/jenkins/results/coverage.xml: Operation not permitted
		at java.base/sun.nio.fs.UnixException.translateToIOException(UnixException.java:100)
		at java.base/sun.nio.fs.UnixException.rethrowAsIOException(UnixException.java:111)
		at java.base/sun.nio.fs.UnixException.rethrowAsIOException(UnixException.java:116)
		at java.base/sun.nio.fs.UnixFileAttributeViews$Posix.setMode(UnixFileAttributeViews.java:254)
		at java.base/sun.nio.fs.UnixFileAttributeViews$Posix.setPermissions(UnixFileAttributeViews.java:276)
		at java.base/java.nio.file.Files.setPosixFilePermissions(Files.java:2080)
		at jenkins.util.io.PathRemover.makeWritable(PathRemover.java:285)
		at jenkins.util.io.PathRemover.makeRemovable(PathRemover.java:258)
		at jenkins.util.io.PathRemover.removeOrMakeRemovableThenRemove(PathRemover.java:238)
		at jenkins.util.io.PathRemover.tryRemoveFile(PathRemover.java:202)
		at jenkins.util.io.PathRemover.tryRemoveRecursive(PathRemover.java:213)
		at jenkins.util.io.PathRemover.tryRemoveDirectoryContents(PathRemover.java:224)
		at jenkins.util.io.PathRemover.tryRemoveRecursive(PathRemover.java:212)
		at jenkins.util.io.PathRemover.tryRemoveDirectoryContents(PathRemover.java:224)
		at jenkins.util.io.PathRemover.tryRemoveRecursive(PathRemover.java:212)
		at jenkins.util.io.PathRemover.tryRemoveDirectoryContents(PathRemover.java:224)
		at jenkins.util.io.PathRemover.forceRemoveDirectoryContents(PathRemover.java:84)
		... 14 more
	Suppressed: java.nio.file.FileSystemException: /var/lib/jenkins/workspace/ne-services_RetailUserOTPFeature/jenkins/results: Operation not permitted
		at java.base/sun.nio.fs.UnixException.translateToIOException(UnixException.java:100)
		at java.base/sun.nio.fs.UnixException.rethrowAsIOException(UnixException.java:111)
		at java.base/sun.nio.fs.UnixException.rethrowAsIOException(UnixException.java:116)
		at java.base/sun.nio.fs.UnixFileAttributeViews$Posix.setMode(UnixFileAttributeViews.java:254)
		at java.base/sun.nio.fs.UnixFileAttributeViews$Posix.setPermissions(UnixFileAttributeViews.java:276)
		at java.base/java.nio.file.Files.setPosixFilePermissions(Files.java:2080)
		at jenkins.util.io.PathRemover.makeWritable(PathRemover.java:285)
		at jenkins.util.io.PathRemover.makeRemovable(PathRemover.java:258)
		at jenkins.util.io.PathRemover.removeOrMakeRemovableThenRemove(PathRemover.java:238)
		at jenkins.util.io.PathRemover.tryRemoveFile(PathRemover.java:202)
		at jenkins.util.io.PathRemover.tryRemoveRecursive(PathRemover.java:213)
		at jenkins.util.io.PathRemover.tryRemoveDirectoryContents(PathRemover.java:224)
		at jenkins.util.io.PathRemover.tryRemoveRecursive(PathRemover.java:212)
		at jenkins.util.io.PathRemover.tryRemoveDirectoryContents(PathRemover.java:224)
		at jenkins.util.io.PathRemover.forceRemoveDirectoryContents(PathRemover.java:84)
		... 14 more
	Suppressed: jenkins.util.io.CompositeIOException: Unable to remove directory /var/lib/jenkins/workspace/ne-services_RetailUserOTPFeature/jenkins with directory contents: [/var/lib/jenkins/workspace/ne-services_RetailUserOTPFeature/jenkins/results]
		at jenkins.util.io.PathRemover.removeOrMakeRemovableThenRemove(PathRemover.java:249)
		at jenkins.util.io.PathRemover.tryRemoveFile(PathRemover.java:202)
		at jenkins.util.io.PathRemover.tryRemoveRecursive(PathRemover.java:213)
		at jenkins.util.io.PathRemover.tryRemoveDirectoryContents(PathRemover.java:224)
		at jenkins.util.io.PathRemover.forceRemoveDirectoryContents(PathRemover.java:84)
		... 14 more
		Suppressed: java.nio.file.DirectoryNotEmptyException: /var/lib/jenkins/workspace/ne-services_RetailUserOTPFeature/jenkins
			at java.base/sun.nio.fs.UnixFileSystemProvider.implDelete(UnixFileSystemProvider.java:247)
			at java.base/sun.nio.fs.AbstractFileSystemProvider.deleteIfExists(AbstractFileSystemProvider.java:110)
			at java.base/java.nio.file.Files.deleteIfExists(Files.java:1181)
			at jenkins.util.io.PathRemover.removeOrMakeRemovableThenRemove(PathRemover.java:236)
			... 18 more
		Suppressed: java.nio.file.DirectoryNotEmptyException: /var/lib/jenkins/workspace/ne-services_RetailUserOTPFeature/jenkins
    
 ```
 
 # solution
``` 
 chown -R jenkins:jenkins /var/lib/jenkins/workspace/jobname
``` 
 
 
