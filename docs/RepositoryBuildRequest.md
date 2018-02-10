# RepositoryBuildRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Subdirectory** | **string** | Subdirectory in which the Dockerfile can be found. You can only specify this or dockerfile_path | [optional] [default to null]
**ArchiveUrl** | **string** | The URL of the .tar.gz to build. Must start with \&quot;http\&quot; or \&quot;https\&quot;. | [optional] [default to null]
**DockerTags** | **[]string** | The tags to which the built images will be pushed. If none specified, \&quot;latest\&quot; is used. | [optional] [default to null]
**PullRobot** | **string** | Username of a Quay robot account to use as pull credentials | [optional] [default to null]
**FileId** | **string** | The file id that was generated when the build spec was uploaded | [optional] [default to null]
**Context** | **string** | Pass in the context for the dockerfile. This is optional. | [optional] [default to null]
**DockerfilePath** | **string** | Path to a dockerfile. You can only specify this or subdirectory. | [optional] [default to null]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


