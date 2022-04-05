# PoolResponse


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tls_ca_cert** | **str, none_type** | A secure certificate to authenticate a server with. Must be in PEM format. | [optional]  if omitted the server will use the default value of "null"
**tls_client_cert** | **str, none_type** | The client certificate used to make authenticated requests. Must be in PEM format. | [optional]  if omitted the server will use the default value of "null"
**tls_client_key** | **str, none_type** | The client private key used to make authenticated requests. Must be in PEM format. | [optional]  if omitted the server will use the default value of "null"
**tls_cert_hostname** | **str, none_type** | The hostname used to verify a server&#39;s certificate. It can either be the Common Name (CN) or a Subject Alternative Name (SAN). | [optional]  if omitted the server will use the default value of "null"
**use_tls** | **int** | Whether to use TLS. | [optional]  if omitted the server will use the default value of 0
**name** | **str** | Name for the Pool. | [optional] 
**shield** | **str, none_type** | Selected POP to serve as a shield for the servers. Defaults to `null` meaning no origin shielding if not set. Refer to the [POPs API endpoint](/reference/api/utils/pops/) to get a list of available POPs used for shielding. | [optional]  if omitted the server will use the default value of "null"
**request_condition** | **str, none_type** | Condition which, if met, will select this configuration during a request. Optional. | [optional] 
**max_conn_default** | **int** | Maximum number of connections. Optional. | [optional]  if omitted the server will use the default value of 200
**connect_timeout** | **int** | How long to wait for a timeout in milliseconds. Optional. | [optional] 
**first_byte_timeout** | **int** | How long to wait for the first byte in milliseconds. Optional. | [optional] 
**quorum** | **int** | Percentage of capacity (`0-100`) that needs to be operationally available for a pool to be considered up. | [optional]  if omitted the server will use the default value of 75
**tls_ciphers** | **str, none_type** | List of OpenSSL ciphers (see the [openssl.org manpages](https://www.openssl.org/docs/man1.1.1/man1/ciphers.html) for details). Optional. | [optional] 
**tls_sni_hostname** | **str, none_type** | SNI hostname. Optional. | [optional] 
**tls_check_cert** | **int, none_type** | Be strict on checking TLS certs. Optional. | [optional] 
**min_tls_version** | **int, none_type** | Minimum allowed TLS version on connections to this server. Optional. | [optional] 
**max_tls_version** | **int, none_type** | Maximum allowed TLS version on connections to this server. Optional. | [optional] 
**healthcheck** | **str, none_type** | Name of the healthcheck to use with this pool. Can be empty and could be reused across multiple backend and pools. | [optional] 
**comment** | **str, none_type** | A freeform descriptive note. | [optional] 
**type** | **str** | What type of load balance group to use. | [optional] 
**override_host** | **str, none_type** | The hostname to [override the Host header](https://docs.fastly.com/en/guides/specifying-an-override-host). Defaults to `null` meaning no override of the Host header will occur. This setting can also be added to a Server definition. If the field is set on a Server definition it will override the Pool setting. | [optional]  if omitted the server will use the default value of "null"
**created_at** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
**deleted_at** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
**updated_at** | **datetime, none_type** | Date and time in ISO 8601 format. | [optional] [readonly] 
**service_id** | **bool, date, datetime, dict, float, int, list, str, none_type** |  | [optional] [readonly] 
**version** | **bool, date, datetime, dict, float, int, list, str, none_type** |  | [optional] [readonly] 
**id** | **bool, date, datetime, dict, float, int, list, str, none_type** |  | [optional] [readonly] 
**any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

