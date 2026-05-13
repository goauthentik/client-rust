# LifecycleIteration

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **uuid::Uuid** |  | [readonly]
**content_type** | [**models::ContentTypeEnum**](ContentTypeEnum.md) |  | 
**object_id** | **String** |  | [readonly]
**object_verbose** | **String** |  | [readonly]
**object_admin_url** | **String** |  | [readonly]
**state** | [**models::LifecycleIterationStateEnum**](LifecycleIterationStateEnum.md) |  | [readonly]
**opened_on** | **chrono::DateTime<chrono::FixedOffset>** |  | [readonly]
**grace_period_end** | **chrono::DateTime<chrono::FixedOffset>** |  | [readonly]
**next_review_date** | **chrono::DateTime<chrono::FixedOffset>** |  | [readonly]
**reviews** | [**Vec<models::Review>**](Review.md) |  | [readonly]
**rule** | [**models::RelatedRule**](RelatedRule.md) |  | [readonly]
**user_can_review** | **bool** |  | [readonly]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


