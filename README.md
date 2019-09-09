# azure-pipelines-environment-variables
Azure DevOps Pipelines CI Windows available environment variables

# Basic terminology

Here are some very basic terms that make understanding the variables easier.

* A **build** is the collection of all the agents, jobs and steps resulting from an event such as submitting a pull request. Depending on how it is configured, a single build may include the use of many different agents, potentially on different operating systems and architectures.
* An **agent** is the process that runs a build on a specific container (i.e., machine). Builds have one or more agents.
* A **job** is a portion of the work to be done by an agent as part of a build. Builds can have zero or more jobs.
* A **step** is a portion of the work to be done by a job. Jobs can have zero or more steps.
* A **task** is a pre-configured step that may require inputs to perform functionality. A task is roughly equivalent to a function call.

# Azure Pipelines Windows Environment Variables

## AGENT_BUILDDIRECTORY

Description: Build directory for the job.

Example: `D:\a\1`

## AGENT_DISABLELOGPLUGIN_TESTFILEPUBLISHERPLUGIN

Description: Disable log plugin test file publisher plugin for the job.

Example: `true`

## AGENT_DISABLELOGPLUGIN_TESTRESULTLOGPLUGIN

Description: Disable log plugin test result log plugin for the job.

Example: `true`

## AGENT_HOMEDIRECTORY

Description: Home directory for the agent.

Example: `C:\agents\2.155.1`

## AGENT_ID

Description: Agent ID.

Example: `78`

## AGENT_JOBNAME

Description: Job display name.

Example: `environment variables`

## AGENT_JOBSTATUS

Description: Status of the job.

Example: `Succeeded`

## AGENT_MACHINENAME

Description: Machine name.

Example: `fv-az433`

## AGENT_NAME

Description: Agent name.

Example: `Hosted Agent`

## AGENT_OS

Description: OS for the job.

Example: `Windows_NT`

## AGENT_OSARCHITECTURE

Description: Whether the agent is running on x64 or x86 architecture.

Example: `X64`

## AGENT_RETAINDEFAULTENCODING

Description: Retain default encoding in job.

Example: `false`

## AGENT_ROOTDIRECTORY

Description: Root directory for the job.

Example: `D:\a`

## AGENT_SERVEROMDIRECTORY

Description: OM directory for the job.

Example: `C:\agents\2.155.1\externals\vstsom`

## AGENT_TEMPDIRECTORY

Description: The agent's temp directory.

Example: `D:\a\_temp`

## AGENT_TOOLSDIRECTORY

Description: Tool's directory.

Example: `C:/hostedtoolcache/windows`

## AGENT_VERSION

Description: The agent version.

Example: `2.155.1`

## AGENT_WORKFOLDER

Description: The agent workfolder.

Example: `D:\a`

## agent.jobstatus

Description: The status of the job.

Example: `Succeeded`

## ALLUSERSPROFILE

Description: Location of all users' profile.

Example: `C:\ProgramData`

## ANDROID_HOME

Description: Android home.

Example: `C:\Program Files (x86)\Android\android-sdk`

## ANDROID_NDK_HOME

Description: Android NDK home.

Example: `C:\Microsoft\AndroidNDK64\android-ndk-r15c`

## ANDROID_NDK_PATH

Description: Android NDK path.

Example: `C:\Microsoft\AndroidNDK64\android-ndk-r15c`

## ANT_HOME

Description: Apache Ant home.

Example: `C:\ProgramData\chocolatey\lib\ant\apache-ant-1.10.5`

## APPDATA

Description: App data directory.

Example: `C:\Users\VssAdministrator\AppData\Roaming`

## AZURE_EXTENSION_DIR

Description: Location of Azure extensions.

Example: `C:\Program Files\Common Files\AzureCliExtensionDirectory`

## AZURE_HTTP_USER_AGENT

Description: HTTP user agent identification.

Example: `VSTS_aea1cc4e-9bc6-4c7b-8950-a47d7d2e4e06_build_2_0`

## BOOST_ROOT_1_69_0

Description: Boost root location for 1.69.0.

Example: `C:\Program Files\Boost\1.69.0`

## BOOST_ROOT

Description: Boost root location.

Example: `C:\Program Files\Boost\1.69.0`

## BUILD_ARTIFACTSTAGINGDIRECTORY

Description: Staging directory for the build artifacts.

Example: `D:\a\1\a`

## BUILD_BINARIESDIRECTORY

Description: Binaries directory for the build.

Example: `D:\a\1\b`

## BUILD_BUILDID

Description: Incrementing number giving build ID.

Example: `64`

## BUILD_BUILDNUMBER

Description: Name given to the build in the `azure-pipelines.yml`. This YAML line resulted in the example below: 

```yaml
name: $(BuildDefinitionName)_$(Date:yyyyMMdd)$(Rev:.rr)
```

Example: `YakDriver.azure-pipelines-environment-variables_20190909.01`

## BUILD_BUILDURI

Description: Build URI.

Example: `vstfs:///Build/Build/64`

## BUILD_CONTAINERID

Description: Container ID.

Example: `4167856`

## BUILD_DEFINITIONNAME

Description: The build definition name (`username.repository_name`).

Example: `YakDriver.azure-pipelines-environment-variables`

## BUILD_DEFINITIONVERSION

Description: The build definition version.

Example: `1`

## BUILD_QUEUEDBY

Description: Whether a user or webhook queued the build. If manually queued, the username will appear, or if queued by webhook from a Git host, e.g., GitHub, that name appears.

Example: `GitHub` or `YakDriver` (username)

## BUILD_QUEUEDBYID

Description: ID of the queueing entity.

Example: `e692fbfb-6e19-6464-9e8d-e2533a449c63`

## BUILD_REASON

Description: Semi-describes reasons for building.

Example: `Manual` or `PullRequest` or `BatchedCI` (merged pull request or new tag)

## BUILD_REPOSITORY_CLEAN

Description: Seems to always be false.

Example: `False`

## BUILD_REPOSITORY_GIT_SUBMODULECHECKOUT

Description: Whether repository submodules are to be checked out.

Example: `False`

## BUILD_REPOSITORY_ID

Description: The ID of the current repository (see `BUILD_REPOSITORY_NAME`).

Example: `YakDriver/azure-pipelines-environment-variables`

## BUILD_REPOSITORY_LOCALPATH

Description: Where the repository was cloned locally.

Example: `D:\a\1\s`

## BUILD_REPOSITORY_NAME

Description: The name of the current repository (see `BUILD_REPOSITORY_ID`).

Example: `YakDriver/azure-pipelines-environment-variables`

## BUILD_REPOSITORY_PROVIDER

Description: The Git host that hosts the current repository.

Example: `GitHub`

## BUILD_REPOSITORY_URI

Description:

Example: `https://github.com/YakDriver/azure-pipelines-environment-variables`

## BUILD_REQUESTEDFOR

Description: Depends on whether manually launched or launched by webhook from, e.g., GitHub.

Example: `GitHub` or `YakDriver` (username)

## BUILD_REQUESTEDFOREMAIL

Description: If launched manually from Azure Pipelines, your associated email address will show up here.

Example: `dirk@example.com`

## BUILD_REQUESTEDFORID

Description:

Example: `e692fbfb-6e19-6464-9e8d-e2533a449c63`

## BUILD_SOURCEBRANCH

Description:

Pull request (PR) example: `refs/pull/1/merge`

Merge pull request, or manual build on a branch example: `refs/heads/master`

Tag example: `refs/tags/v0.1.0`

## BUILD_SOURCEBRANCHNAME

Description: This does not always contain the branch name, such as on a pull request, when it contains `merge`. If the build corresponds to a new tag, this contains the new tag name.

Pull request (PR) example: `merge`

Merge pull request, or manual build on a branch example: `master`

Tag example: `v0.1.0`

## BUILD_SOURCESDIRECTORY

Description:

Example: `D:\a\1\s`

## BUILD_SOURCEVERSION

Description: Current Git hash of the target branch.

Example: `6451d5a2ea8f90ff2453dc8d9b434d545041166d`

## BUILD_SOURCEVERSIONAUTHOR

Description:

Example: `Dirk Avery`

## BUILD_SOURCEVERSIONMESSAGE

Description: For a pull request, this provides the Git hashes - the hash of the current commit and the hash of the branch head where the commit would be merged. On a manual build on a branch, this contains the commit message.

Pull request (PR) example: `Merge 4072182801f9d627f33593f2b0f38924d365cd0f into 6451d5a2ea8f90ff2453dc8d9b434d545041166d`

Manual build on a branch example: `Add ap yaml file` (Git commit message)

Tag example: `Merge pull request #1 from YakDriver/update-envs`

## BUILD_STAGINGDIRECTORY

Description:

Example: `D:\a\1\a`

## ChocolateyInstall

Description:

Example: `C:\ProgramData\chocolatey`

## ChromeWebDriver

Description:

Example: `C:\SeleniumWebDrivers\ChromeDriver`

## COBERTURA_HOME

Description:

Example: `C:\cobertura-2.1.1`

## COMMON_TESTRESULTSDIRECTORY

Description:

Example: `D:\a\1\TestResults`

## CommonProgramFiles(x86)

Description:

Example: `C:\Program Files (x86)\Common Files`

## COMMONPROGRAMFILES

Description: _(Camel case on CMD and PowerShell.)_

Example: `C:\Program Files\Common Files`

## CommonProgramW6432

Description:

Example: `C:\Program Files\Common Files`

## COMPUTERNAME

Description:

Example: `fv-az433`

## COMSPEC

Description: _(Camel case on CMD and PowerShell.)_

Example: `C:\windows\system32\cmd.exe`

## CONDA

Description:

Example: `C:\Miniconda`

## ENDPOINT_URL_SYSTEMVSSCONNECTION

Description: _(Bash only.)_

Example: `https://dev.azure.com/yakdriver/`

## EXEPATH

Description: _(Bash only.)_

Example: `C:\Program Files\Git\bin`

## GeckoWebDriver

Description:

Example: `C:\SeleniumWebDrivers\GeckoDriver`

## GIT_TERMINAL_PROMPT

Description:

Example: `0`

## GOROOT_1_10_X64

Description:

Example: `C:\Go1.10.8`

## GOROOT_1_11_X64

Description:

Example: `C:\Go1.11.12`

## GOROOT_1_12_X64

Description:

Example: `C:\Go1.12.7`

## GOROOT_1_9_X64

Description:

Example: `C:\Go1.9.7`

## GOROOT

Description:

Example: `C:\Go1.12.7`

## GRADLE_HOME

Description:

Example: `C:\ProgramData\chocolatey\lib\gradle\tools\gradle-5.6`

## HOME

Description: _(Bash only.)_

Example: `/c/Users/VssAdministrator`

## HOMEDRIVE

Description:

Example: `C:`

## HOMEPATH

Description:

Example: `\Users\VssAdministrator`

## IEWebDriver

Description:

Example: `C:\SeleniumWebDrivers\IEDriver`

## ImageVersion

Description:

Example: `157.1`

## INPUT_ARGUMENTS

Description: _(Bash only, arguments to the `env` command.)_

Example: ``

## JAVA_HOME_11_X64

Description:

Example: `C:\Program Files\Java\zulu-11-azure-jdk_11.33.15-11.0.4-win_x64`

## JAVA_HOME_7_X64

Description:

Example: `C:\Program Files\Java\zulu-7-azure-jdk_7.31.0.5-7.0.232-win_x64`

## JAVA_HOME_8_X64

Description:

Example: `C:\Program Files\Java\zulu-8-azure-jdk_8.40.0.25-8.0.222-win_x64`

## JAVA_HOME

Description:

Example: `C:\Program Files\Java\zulu-8-azure-jdk_8.40.0.25-8.0.222-win_x64`

## LOCALAPPDATA

Description:

Example: `C:\Users\VssAdministrator\AppData\Local`

## LOGONSERVER

Description:

Example: `\\fv-az433`

## M2_HOME

Description:

Example: `C:\ProgramData\chocolatey\lib\maven\apache-maven-3.6.1`

## M2_REPO

Description:

Example: `C:\ProgramData\m2`

## M2

Description:

Example: `\bin`

## MAVEN_OPTS

Description:

Example: `-Xms256m`

## MSDEPLOY_HTTP_USER_AGENT

Description:

Example: `VSTS_aea1cc4e-9bc6-4c7b-8950-a47d7d2e4e06_build_2_0`

## MSMPI_BIN

Description:

Example: `C:\Program Files\Microsoft MPI\Bin\`

## MSYSTEM

Description: _(Bash only.)_

Example: `MINGW64`

## NPM_CONFIG_CACHE

Description:

Example: `C:\npm\cache`

## NPM_CONFIG_PREFIX

Description:

Example: `C:\npm\prefix`

## NUMBER_OF_PROCESSORS

Description:

Example: `2`

## OS

Description:

Example: `Windows_NT`

## PATH

Description: _(Camel case on CMD and PowerShell.)_

Bash example: `/mingw64/bin:/usr/bin:/c/Users/VssAdministrator/bin:/c/agents/2.155.1/externals/git/cmd...`

CMD and PowerShell example: `Path=C:\agents\2.155.1\externals\git\cmd;C:/hostedtoolcache/windows\Python\3.6.8\x64;C:/hostedtoolcache/windows\Python\3.6.8\x64\Scripts;C:\Program Files\Mercurial\;C:\vcpkg;C:\cf-cli;C:\Program Files (x86)\NSIS\;C:\Program Files\Mercurial\;C:\Program Files\Boost\1.69.0...`

## PATHEXT

Description:

Example: `.COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC;.PY`

## PHPROOT

Description:

Example: `c:\tools\php`

## PIPELINE_WORKSPACE

Description:

Example: `D:\a\1`

## PLINK_PROTOCOL

Description: _(Bash only.)_

Example: `ssh`

## PROCESSOR_ARCHITECTURE

Description:

Example: `AMD64`

## PROCESSOR_IDENTIFIER

Description:

Example: `Intel64 Family 6 Model 79 Stepping 1, GenuineIntel`

## PROCESSOR_LEVEL

Description:

Example: `6`

## PROCESSOR_REVISION

Description:

Example: `4f01`

## ProgramData

Description:

Example: `C:\ProgramData`

## ProgramFiles(x86)

Description:

Example: `C:\Program Files (x86)`

## PROGRAMFILES

Description: _(Camel case on CMD and PowerShell.)_

Example: `C:\Program Files`

## ProgramW6432

Description:

Example: `C:\Program Files`

## PROMPT

Description: _(CMD only.)_

Example: `$P$G`

## PSModulePath

Description:

Example: `C:\Modules\azurerm_2.1.0;C:\Modules\azure_2.1.0;C:\Users\packer\Documents\WindowsPowerShell\Modules;C:\Program Files\WindowsPowerShell\Modules;C:\windows\system32\WindowsPowerShell\v1.0\Modules;C:\Program Files\Microsoft SQL Server\130\Tools\PowerShell\Modules\`

## PSExecutionPolicyPreference

Description: _(CMD and PowerShell only.)_

Example: `Unrestricted`

## PUBLIC

Description:

Example: `C:\Users\Public`

## PWD

Description:

Example: `/d/a/1/s`

## PYTHON_HOME

Description:

Example: `C:/hostedtoolcache/windows\Python\3.6.8\x64`

## RUNNER_TOOLSDIRECTORY

Description:

Example: `C:/hostedtoolcache/windows`

## SHLVL

Description: _(Bash only.)_

Example: `1`

## SYSTEM_ARTIFACTSDIRECTORY

Description:

Example: `D:\a\1\a`

## SYSTEM_COLLECTIONID

Description:

Example: `aea1cc4e-9bc6-4c7b-8950-a47d7d2e4e06`

## SYSTEM_COLLECTIONURI

Description:

Example: `https://dev.azure.com/yakdriver/`

## SYSTEM_CULTURE

Description:

Example: `en-US`

## SYSTEM_DEFAULTWORKINGDIRECTORY

Description:

Example: `D:\a\1\s`

## SYSTEM_DEFINITIONID

Description:

Example: `2`

## SYSTEM_DEFINITIONNAME

Description:

Example: `YakDriver.azure-pipelines-environment-variables`

## SYSTEM_ENABLEACCESSTOKEN

Description:

Example: `SecretVariable`

## SYSTEM_HOSTTYPE

Description:

Example: `build`

## SYSTEM_ISSCHEDULED

Description:

Example: `False`

## SYSTEM_JOBATTEMPT

Description:

Example: `1`

## SYSTEM_JOBDISPLAYNAME

Description:

Example: `environment variables`

## SYSTEM_JOBID

Description:

Example: `9cd7d73b-785a-5059-5c5c-3f86b8afeb34`

## SYSTEM_JOBIDENTIFIER

Description:

Example: `env.__default`

## SYSTEM_JOBNAME

Description:

Example: `__default`

## SYSTEM_JOBPARALLELISMTAG

Description:

Example: `Public`

## SYSTEM_JOBPOSITIONINPHASE

Description:

Example: `1`

## SYSTEM_PHASEATTEMPT

Description:

Example: `1`

## SYSTEM_PHASEDISPLAYNAME

Description:

Example: `environment variables`

## SYSTEM_PHASEID

Description:

Example: `37905b85-ba64-57a9-b162-719366a83dda`

## SYSTEM_PHASENAME

Description:

Example: `env`

## SYSTEM_PIPELINESTARTTIME

Description:

Example: `2019-09-09 15:12:39-04:00`

## SYSTEM_PLANID

Description:

Example: `50e3405c-d780-4774-8541-b0fdb2b26341`

## SYSTEM_PULLREQUEST_ISFORK

Description: Even though pull request related, this appears in non-pull-request builds.

Example: `False`

## SYSTEM_PULLREQUEST_MERGEDAT

Description: _Only on a pull request._

Example: ``

## SYSTEM_PULLREQUEST_PULLREQUESTID

Description: _Only on a pull request._

Example: `315675853`

## SYSTEM_PULLREQUEST_PULLREQUESTNUMBER

Description: _Only on a pull request._

Example: `1`

## SYSTEM_PULLREQUEST_SOURCEBRANCH

Description: _Only on a pull request._

Example: `update-envs`

## SYSTEM_PULLREQUEST_SOURCECOMMITID

Description: _Only on a pull request._

Example: `4072182801f9d627f33593f2b0f38924d365cd0f`

## SYSTEM_PULLREQUEST_SOURCEREPOSITORYURI

Description: _Only on a pull request._

Example: `https://github.com/YakDriver/azure-pipelines-environment-variables.git`

## SYSTEM_PULLREQUEST_TARGETBRANCH

Description: _Only on a pull request._

Example: `master`

## SYSTEM_SERVERTYPE

Description:

Example: `Hosted`

## SYSTEM_STAGEATTEMPT

Description: 

Example: `1`

## SYSTEM_STAGEDISPLAYNAME

Description: The display name for the stage.

Example: `__default`

## SYSTEM_STAGEID

Description: A UUID for the current stage.

Example: `96ac2280-8cb4-5df5-99de-dd2da759617d`

## SYSTEM_STAGENAME

Description: The stage name.

Example: `__default`

## SYSTEM_TASKDEFINITIONSURI

Description: The URI for the step definitions.

Example: `https://dev.azure.com/yakdriver/`

## SYSTEM_TASKDISPLAYNAME

Description: The display name for the current step.

Example: `bash environment variables`

## SYSTEM_TASKINSTANCEID

Description: A UUID for the current step.

Example: `ce30c491-54d2-5ab2-f73d-c2aceaff5b23`

## SYSTEM_TASKINSTANCENAME

Description: What type of step is currently running.

Example: `Bash`

## SYSTEM_TEAMFOUNDATIONCOLLECTIONURI

Description: The collection URI for the Team Foundation Server (now Azure DevOps Server).

Example: `https://dev.azure.com/yakdriver/`

## SYSTEM_TEAMFOUNDATIONSERVERURI

Description: The URI for the Team Foundation Server (now Azure DevOps Server).

Example: `https://dev.azure.com/yakdriver/`

## SYSTEM_TEAMPROJECT

Description: The team project.

Example: `dirkavery`

## SYSTEM_TEAMPROJECTID

Description: A UUID for the team project.

Example: `e556bba9-d99e-42da-baad-6ed357d52dcf`

## SYSTEM_TIMELINEID

Description: A UUID for the system timeline.

Example: `50e3405c-d780-4774-8541-b0fdb2b26341`

## SYSTEM_TOTALJOBSINPHASE

Description: How many parallel jobs are in phase.

Example: `1`

## SYSTEM_WORKFOLDER

Description: The system workfolder.

Example: `D:\a`

## SYSTEM

Description: The purpose of the system perhaps.

Example: `build`

## SYSTEMDRIVE

Description: _(Camel case on CMD and PowerShell.)_ The drive where the system lives.

Example: `C:`

## SYSTEMROOT

Description: _(Camel case on CMD and PowerShell.)_ The Windows system root.

Example: `C:\windows`

## TASK_DISPLAYNAME

Description: The display name of the current task.

Example: `bash environment variables`

## TEMP

Description: The location of temporary directory.

Bash example: `/tmp`

CMD and PowerShell example: `C:\Users\VSSADM~1\AppData\Local\Temp`

## TERM

Description: _(Bash only.)_ The terminal emulator.

Example: `cygwin`

## TF_BUILD

Description: Whether this is a Team Foundation (now Azure DevOps) build.

Example: `True`

## TMP

Description: The location of temporary directory.

Bash Example: `/tmp`

CMD and PowerShell example: `C:\Users\VSSADM~1\AppData\Local\Temp`

## USER_DEFINED_VARIABLE

Description: If you have a job or build-level user-defined variable, it will show up in the environment as well. This is an example.

Example: `the value of this variable`

## USERDOMAIN_ROAMINGPROFILE

Description: The roaming profile in the domain.

Example: `fv-az433`

## USERDOMAIN

Description: The domain of the container.

Example: `fv-az433`

## USERNAME

Description: The username running the build.

Example: `VssAdministrator`

## USERPROFILE

Description: The user profile location.

Example: `C:\Users\VssAdministrator`

## VCPKG_INSTALLATION_ROOT

Description: The VCPKG installation root.

Example: `C:\vcpkg`

## VS140COMNTOOLS

Description: The location of VS140 common tools.

Example: `C:\Program Files (x86)\Microsoft Visual Studio 14.0\Common7\Tools\`

## VSTS_AGENT_PERFLOG

Description: The VSTS agent performance log.

Example: `c:\vsts\perflog`

## VSTS_PROCESS_LOOKUP_ID

Description: The lookup ID of the VSTS process.

Example: `vsts_d35522da-a32f-41c8-bded-bc0b6eaf1530`

## WINDIR

Description: _(Lowercase on CMD and PowerShell.)_ The location of Windows.

Example: `C:\windows`

## WIX

Description: The location of WiX.

Example: `C:\Program Files (x86)\WiX Toolset v3.11\`
