# Experience API
## Advanced Distributed Learning (ADL) Co-Laboratories

>#### License

>"Copyright 2013 Advanced Distributed Learning (ADL) Initiative, U.S. Department of Defense

>Licensed under the Apache License, Version 2.0 (the "License"). You may not use this file except 
>in compliance with the License. You may obtain a copy of the License at
>http://www.apache.org/licenses/LICENSE-2.0

>Unless required by applicable law or agreed to in writing, software distributed under the License 
>is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express 
>or implied. See the License for the specific language governing permissions and limitations under 
>the License."

>This document was authored by members of the Experience API Working Group (see 
>list in [CONTRIBUTING.md](CONTRIBUTING.md#contributors)) in support of the Office of the Deputy Assistant Secretary of 
>Defense (Readiness) Advanced Distributed Learning (ADL) Initiative. Please 
>send all feedback and inquiries to helpdesk@adlnet.gov  

## Table of Contents
*	Part One:	[About the Experience API](./xAPI-About.md#partone)  
	*	1.0.	[Introduction](./xAPI-About.md#introduction-partone) 
	*	2.0.	[How To Use This Document](./xAPI-About.md#readingguidelines)  
		*	2.1.	[MUST / SHOULD / MAY](./xAPI-About.md#def-must-should-may)  
	 	*	2.2.	[Guidelines for Interpreting Descriptive Text and Tables](./xAPI-About.md#interpret-text-table)  
	*	3.0.	[Serialization and JavaScript Object Notation](./xAPI-About.md#json)
	*	4.0.	[Definitions](./xAPI-About.md#definitions) 
	*	5.0.	[xAPI Components](./xAPI-About.md#xapi-components) 
	*	6.0.	[Extending xAPI](./xAPI-About.md#extending-xapi) 
	*	7.0.	[Profiles and Communities of Practice](./xAPI-About.md#COPs)  
	*	[Appendices](./xAPI-About.md#append1)  
		*	[Appendix A: Revision History](./xAPI-About.md#Appendix1A)  
		*	[Appendix B: cmi5 Example](./xAPI-About.md#Appendix1B)  
*	Part Two:	[Experience API Data](./xAPI-Data.md#parttwo)  
	*	1.0.	[Documents](./xAPI-Data.md#documents) 
	*	2.0.	[Statements](./xAPI-Data.md#statements)  
		*	2.1.	[Purpose](./xAPI-Data.md#statement-purpose)  
	 	*	2.2.	[Formatting Requirements](./xAPI-Data.md#dataconstraints) 
	 	*	2.3.	[Statement Lifecycle](./xAPI-Data.md#lifecycle) 
		 	*	2.3.1.	[Statement Immutability](./xAPI-Data.md#statement-immutability-and-exceptions) 
		 	*	2.3.2.	[Voiding](./xAPI-Data.md#voided) 
   		*	2.4.	[Statement Properties](./xAPI-Data.md#statement-properties)  
	        *	2.4.1.	[ID](./xAPI-Data.md#stmtid)  
	        *	2.4.2.	[Actor](./xAPI-Data.md#actor)  
	        *	2.4.3.	[Verb](./xAPI-Data.md#verb)  
	        *	2.4.4.	[Object](./xAPI-Data.md#object)  
	        *	2.4.5.	[Result](./xAPI-Data.md#result)  
	        *	2.4.6.	[Context](./xAPI-Data.md#context)  
	        *	2.4.7.	[Timestamp](./xAPI-Data.md#timestamp)  
	        *	2.4.8.	[Stored](./xAPI-Data.md#stored)  
	        *	2.4.9.	[Authority](./xAPI-Data.md#authority)  
	        *	2.4.10.	[Version](./xAPI-Data.md#version)  
	        *	2.4.11.	[Attachments](./xAPI-Data.md#attachments)  
    	*	2.5.	[Retrieval of Statements](./xAPI-Data.md#retrieval)   
    	*	2.6.	[Signed Statements](./xAPI-Data.md#signature)  
	*	3.0.	[Metadata](./xAPI-Data.md#metadata)
		*	3.1.	[IRI Requirements](./xAPI-Data.md#iri-requirements)  
		*	3.2.	[Hosted Metadata](./xAPI-Data.md#miscmeta)  
    *	4.0.	[Special Data Types and Rules](./xAPI-Data.md#special-data)  
		*	4.1.	[Extensions](./xAPI-Data.md#miscext) 
		*	4.2.	[Language Maps](./xAPI-Data.md#lang-maps)
		*	4.3.	[IRIs](./xAPI-Data.md#iris)
		*	4.4.	[UUIDs](./xAPI-Data.md#uuids)
		*	4.5.	[ISO 8601 Timestamps](./xAPI-Data.md#timestamps)
		*	4.6.	[ISO 8601 Durations](./xAPI-Data.md#durations)
	*	[Appendices](./xAPI-Data.md#append2)  
		*	[Appendix A: Example Statements](./xAPI-Data.md#Appendix2A)  
		*	[Appendix B: Example statement objects of different types](./xAPI-Data.md#Appendix2B)  
		*	[Appendix C: Example definitions for Activities of type "cmi.interaction"](./xAPI-Data.md#Appendix2C)  	
		*	[Appendix D: Example Signed Statement](./xAPI-Data.md#Appendix2D)  
*	Part Three:	[Data Processing, Validation, and Security](./xAPI-Communication.md#partthree)  
	*	1.0.	[Requests](./xAPI-Communication.md#requests)
		*	1.1.	[HEAD Request Implementation](./xAPI-Communication.md#httphead)  
	 	*	1.2.	[Headers](./xAPI-Communication.md#headers) 
	 	*	1.3.	[Alternate Request Syntax](./xAPI-Communication.md#alt-request-syntax) 
	 	*	1.4.	[Encoding](./xAPI-Communication.md#encoding) 
	 	*	1.5.	[Content Types](./xAPI-Communication.md#content-types) 
	        *	1.5.1.	[Application/JSON](./xAPI-Communication.md#applicationjson) 
	        *	1.5.2.	[Multipart/Mixed](./xAPI-Communication.md#multipartmixed)
	*	2.0.	[Resources](./xAPI-Communication.md#datatransfer)   
	 	*	2.1.	[Statement Resource](./xAPI-Communication.md#stmtres) 
	 	*	2.2.	[Documents Resources](./xAPI-Communication.md#doctransfer) 
	 	*	2.3.	[State Resource](./xAPI-Communication.md#stateres) 
	 	*	2.4.	[Agents Resource](./xAPI-Communication.md#agentsres) 
	 	*	2.5.	[Activities Resource](./xAPI-Communication.md#activitiesres) 
	 	*	2.6.	[Agent Profile Resource](./xAPI-Communication.md#agentprofres) 
	 	*	2.7.	[Activity Profile Resource](./xAPI-Communication.md#actprofres) 
	 	*	2.8.	[About Resource](./xAPI-Communication.md#aboutresource) 
   	*	3.0.	[Data Validation](./xAPI-Communication.md#validation)     
    	*	3.1.	[Concurrency](./xAPI-Communication.md#concurrency)  
    	*	3.2.	[Error Codes](./xAPI-Communication.md#errorcodes)
    	*	3.3     [Versioning](./xAPI-Communication.md#versioning)  
    *	4.0.	[Authentication](./xAPI-Communication.md#authentication)  
		*	4.1.	[OAuth 1.0 Authentication Scenarios and Methods](./xAPI-Communication.md#authdefs) 
		*	4.2.	[OAuth 1.0 Authorization Scope](./xAPI-Communication.md#oauthscope)
    *	5.0	[Security](./xAPI-Communication.md#security)
	*	[Appendices](./xAPI-Communication.md#append3)  
		*	[Appendix A: Converting Statements to 1.0.0](./xAPI-Communication.md#Appendix3A)  
		*	[Appendix B: Table of All Resources](./xAPI-Communication.md#Appendix3B)  
		*	[Appendix C: Cross Domain Request Example](./xAPI-Communication.md#Appendix3C)  

<a name="partthree" />
# Part Three: Data Processing, Validation, and Security 第三部分 数据的传输，验证，和安全

第三部分更详细介绍了xAPI的技术方面，在学习记录提供者和LRS之间传送语句是如何处理的。许多用于处理的函数库（包括JavaScript）在这里被详细说明。因此，学习记录提供者可能不需要完全理解本规范的这一部分的每一个细节。

<a name="requests"/>

## <a name="1.0">1.0</a> Requests 请求

XAPI 追踪是通过由学习记录提供者（客户端）向LRS（服务端）发送HTTP请求来实现的。这一部分将集中于两者之间的交流上。说明里没有规范的，请用当下行业最好的方法习惯来申明

<a name="httphead"/>

### <a name="1.1">1.1</a> HEAD Request Implementation HEAD 请求申明

###### <a name="1.1.s1"></a>Description 描述

对于LRS 的PUT,POST,GET和DELETE请求都在后文有详细说明。。。，所有的说明都支持GET请求也支持HEAD。LRS对HEAD请求只会返回元信息，使用HTTP头文件，而不是真正的文档。 

###### <a name="1.1.s2"></a>Rationale 缘由

访问LRS的客户端可能需要检查特定语句是否存在，或者确定文档的修改日期，例如状态，活动配置文件或代理配置文件资源中的文档。特别是对于大型文档，更有效的是不检索整个文档以检查其修改日期

###### <a name="1.1.s3"></a>LRS Requirements 对LRS的要求
* <a name="1.1.s3.b1"></a>LRS必须响应任何HTTP HEAD请求，因为它将响应一个相同的HTTP GET请求，除下列情况：
    * <a name="1.1.s3.b1.b1"></a>消息的部分必须被忽略时
    * <a name="1.1.s3.b1.b2"></a>内容长度头部可以被省略，以避免浪费LRS资源

<a name="headers"/> 

### <a name="1.2">1.2</a> Headers 头报

##### <a name="1.2.s1"></a>Header Parameters 头参数

在xAPI数据传输中使用的一些头参数是[standard HTTP headers 标准HTTP头](http://en.wikipedia.org/wiki/List_of_HTTP_header_fields)。其他的于此规范中描述。在本规范中描述的一些或所有类型的请求和情况下，期望学习记录提供者使用以下请求参数：

* <a name="1.2.s1.b1"></a>Accept
* <a name="1.2.s1.b2"></a>Accept-Encoding
* <a name="1.2.s1.b3"></a>Accept-Language
* <a name="1.2.s1.b4"></a>Authorization
* <a name="1.2.s1.b5"></a>Content-Type
* <a name="1.2.s1.b6"></a>Content-Length
* <a name="1.2.s1.b7"></a>Content-Transfer-Encoding
* <a name="1.2.s1.b8"></a>If-Match
* <a name="1.2.s1.b9"></a>If-None-Match
* <a name="1.2.s1.b10"></a>X-Experience-API-Version 

LRS返回的头文件应当如下，再次申明，不是所有的类型的请求和情景都需要全部申明这些参数

* <a name="1.2.s1.b11"></a>Content-Type
* <a name="1.2.s1.b12"></a>Content-Length
* <a name="1.2.s1.b13"></a>Last-Modified
* <a name="1.2.s1.b14"></a>ETag
* <a name="1.2.s1.b15"></a>Status
* <a name="1.2.s1.b16"></a>X-Experience-API-Version
* <a name="1.2.s1.b17"></a>X-Experience-API-Consistent-Through

以上列出的不旨在详尽，更多详细信息参见后文

<a name="alt-request-syntax"/>

### <a name="1.3">1.3</a> Alternate Request Syntax 备用请求标签


###### <a name="1.3.s1"></a>Description 描述

xAPI的目标之一是允许跨域跟踪，即使xAPI试图启用除浏览器之外的应用程序进行跟踪，仍需要支持浏览器。例如，Internet Explorer 8和9不实施跨源资源共享，而是使用它们自己的跨域请求API，由于仅支持“GET”和“POST”，所以其不能使用如上所述的所有xAPI，也不允许设置HTTP头。

###### <a name="1.3.s2"></a>Details/Requirements 详情，要求
下列标签，尽量在不能使用常规标签实现的情况下才使用。这些标签也能在GET语句中使用，由于对查询字符串长度的限制，这些可选标签也可用于GET语句。

例子参见 [Appendix C: Cross Domain Request Example](#Appendix3C) 

###### <a name="1.3.s3"></a>Requirements

__Method__:  
* <a name="1.3.s3.b1"></a>所有的xAPI请求情形必须MUST 为POST 
* <a name="1.3.s3.b2"></a>“method”查询字符串参数的值必须是预期的xAPI方法。
* <a name="1.3.s3.b3"></a>学习记录提供者MUST NOT 不能包含任何查询字符串参数在请求里

例子: http://example.com/xAPI/statements?method=PUT 

__Content 内容__:  
* <a name="1.3.s3.b4"></a>如果xAPI请求包含传输内容，那么LRP必须MUST将内容进行URL编码然后放到一个为“content”的参数中
* <a name="1.3.s3.b5"></a>LRS MUST 必须将内容以UTF-8编码，存储二进制数据不被这个标签所支持。

__Headers 头部__:  
* <a name="1.3.s3.b6"></a>学习记录提供者可以包括本规范所要求的任何头参数，它们预期作为具有相同名称的表单参数出现在HTTP头中。这适用于以下参数：Authorization, X-Experience-API-Version, Content-Type, Content-Length, If-Match and If-None-Match. 不适用于 Content-Transfer-Encoding
* <a name="1.3.s3.b7"></a>LRS MUST 必须将上述形式参数视为头参数
* <a name="1.3.s3.b8"></a>学习记录提供者必须MUST必须将其余的没有列出的HTTP头参数正常包含于HTTP头中
* <a name="1.3.s3.b9"></a>学习记录提供者SHOULD*应当依然要包含一个值为'application/x-www-form-urlencoded'的Content-Length头（在HTTP头中）对于这种类型的请求
* <a name="1.3.s3.b10"></a>Content-Type形式参数SHOULD*应当明确内容的类型
* <a name="1.3.s3.b11"></a>学习记录提供者应当SHOULD*为这种类型的请求包括用于指示请求的内容的总长度的Content-Length头部（在HTTP头中）。 
* <a name="1.3.s3.b12"></a>Content-Length形式参数应当SHOULD *指定内容表单参数中内容的长度，因此将比Content-Length标头中列出的长度更低

__Query string parameters 查询字符参数组__:  
* <a name="1.3.s3.b13"></a>除“method”之外的任何查询字符串参数务必包含为具有相同名称的形式参数。
* <a name="1.3.s3.b14"></a>LRS必须处理除“content”或上面列出的头参数以外的任何作为查询字符串参数的形式参数。 

__Attachments__: 由于编码的原因，不能传输二进制。参见 [Attachments](./xAPI-Data.md#attachments) 

* <a name="1.3.s3.b15"></a>LRS必须MUST支持上述句法

可能存在这样的情况，即学习记录提供者需要支持应用程序或浏览器，其中客户端代码托管在来自LRS的不同方案（HTTP或HTTPS）上。只有当你想支持来自IE 9或更低版本的HTTP到HTTPS请求时，才需要代理。如果使用现代浏览器，您可以在不使用代理的情况下执行HTTP到HTTPS（或HTTPS到HTTP！）。两个简单的解决方案可能是1）在与客户端代码相同的方案上建立代理通过到LRS或2）在与客户端代码相同的方案上托管中间服务器端LRS以将语句路由到目标LRS。

在使用HTTP请求时请充分考虑安全因素

<a name="encoding"/> 

### <a name="1.4">1.4</a> Encoding 编码

###### <a name="1.4.s1"></a>Requirements 
* <a name="1.4.s1.b1"></a>所有的文本必须MUST使用UTF-8

<a name="content-types"/> 
### <a name="1.5">1.5</a> Content Types
在请求和响应中一般使用 `application/json` ，例外的情况如下：

* <a name="1.5.b1"></a>文档可以有任何类型
* <a name="1.5.b2"></a>有着附件的语句请求有时候使用 `multipart/mixed`类型 

<a name="applicationjson"/> 
#### <a name="1.5.1">1.5.1</a> Application/JSON
一般使用的内容类型`application/json`

###### <a name="1.5.1.s1"></a>LRS Requirements 对LRS的要求
* <a name="1.5.1.s1.b1"></a>当接受到有着类型为`application/json`的PUT或者POST请求时，LRS 必须MUST 接受不包含附件对象的语句批处理 
* <a name="1.5.1.s1.b2"></a>当接受到有着类型为`application/json`的PUT或者POST请求时，LRS 必须MUST 接受只包含附件对象的处理

<a name="multipartmixed"/> 
#### <a name="1.5.2">1.5.2</a> Multipart/Mixed

`multipart/mixed`内容类型用于可能包含“附件”的请求。这并不意味着所有的“multipart / mixed”请求都必须包含附件。

##### <a name="1.5.2.s1"></a>Procedure For The Exchange Of Attachments 附件交互的过程

* <a name="1.5.2.s1.b1"></a>对于附件为零或者更多的的语句的描述参见前文
* <a name="1.5.2.s1.b2"></a>语句使用内容类型 `multipart/mixed`任何附件都必须放在传输的结尾.

* <a name="1.5.2.s1.b3"></a>LRS可以决定接受或者拒绝这样的语句

* <a name="1.5.2.s1.b4"></a>如果它接受请求，它可以通过将原始数据的SHA-2与在报头中声明的SHA-2进行比较，来将附件的原始数据与附件头匹配

###### <a name="1.5.2.s2"></a>Requirements for Attachment Statement Batches 对于附件语句批的要求

发送包含附件的语句批处理，语句结果或单个语句的请求必须满足以下条件之一：

* <a name="1.5.2.s2.b1"></a>对于任何一个附件必须包含类型为`application/json`，和有一个fileUrl除非"attachments" 过滤的结果为`false`
* <a name="1.5.2.s2.b2"></a>它必须满足“multipart/mixed”在[RFC 2046](https://www.ietf.org/rfc/rfc2046.txt)中的定义
    * <a name="1.5.2.s2.b2.b1"></a>这个多部分文档的第一部分类型必须为 `application/json`.
    * <a name="1.5.2.s2.b2.b2"></a>针对语句资源发出PUT或POST请求，每个附加部分包含附件的原始数据，并构成语句的逻辑部分时，此功能将可用
    * <a name="1.5.2.s2.b2.b3"></a>必须在第一个（语句）部分之后的每个部分的头中包含X-Experience-API-Hash参数。
    * <a name="1.5.2.s2.b2.b4"></a>必须包含一个Content-Transfer-Encoding参数，在第一个（语句）部分后面的每个部分的头部中具有二进制`binary`值 
    * <a name="1.5.2.s2.b2.b5"></a>当在一起发送的多个语句中使用相同的附件时，应仅包含附件数据的一个副本。
    * <a name="1.5.2.s2.b2.b6"></a>应在每个部件的标题中包含一个Content-Type参数。对于第一部分（包含Statement），这必须是 `application/json`.
   	* <a name="1.5.2.s2.b2.b7"></a>如果参数在附件对象（上表中概述）中具有相应的属性，并且为给定的附件指定了参数和属性，则这些参数和属性的值必须匹配。

###### <a name="1.5.2.s3"></a>LRS Requirements 对LRS的要求
* <a name="1.5.2.s3.b1"></a>当客户要求时，LRS必须包括上述传输格式的附件（见语句资源） (see [Statement Resource](#stmtres)).
* <a name="1.5.2.s3.b2"></a>一个LRS不得从另一个LRS中删除语句，而不请求附件。
* <a name="1.5.2.s3.b3"></a>LRS不得将语句推入另一个LRS 
* <a name="1.5.2.s3.b4"></a>当接收到具有`multipart/mixed`的文档类型的PUT或POST时，LRS必须接受包含上述传输格式中的附件的批量语句。
* <a name="1.5.2.s3.b5"></a>当接收到具有`multipart/mixed`的文档类型的PUT或POST时，LRS必须拒绝具有不包含fileUrl的附件的语句批次，也不会基于它们的散列匹配接收到的附件部分。
* <a name="1.5.2.s3.b6"></a>当接收到一个文档类型为`multipart/mixed`的PUT或POST时，LRS应该假设Content-Transfer-Encoding部分是二进制编码。
* <a name="1.5.2.s3.b7"></a>LRS可以拒绝（批）大于LRS语句配置允许数量的批
* <a name="1.5.2.s3.b8"></a>当接收到具有`multipart/mixed`的文档类型的PUT或POST时，LRS应该接受不包含附件对象的语句批次。
* <a name="1.5.2.s3.b9"></a>当接收到具有`multipart/mixed`的文档类型的PUT或POST时，LRS应该接受只包含具有填充的fileUrl的附件对象的批量语句。

__Note:__ 对于使用“mime / multipart”格式的语句批处理包含的附件没有要求。

###### <a name="1.5.2.s4"></a>Learning Record Provider Requirements 对于学习记录提供者的要求
* <a name="1.5.2.s4.b1"></a>学习记录提供者可以如上所述发送具有附件的语句。
* <a name="1.5.2.s4.b2"></a>学习记录提供者可以发送多个语句，其中一些或全部具有附件，如果使用POST。
* <a name="1.5.2.s4.b3"></a>学习记录提供者可以发送`application/json`类型的批次，其中每个附件对象都有一个fileUrl，忽略基于"multipart/mixed"格式的所有要求
* <a name="1.5.2.s4.b4"></a>学习记录提供者应该使用SHA-256，SHA-384和SHA-512填充“sha2”属性

###### <a name="1.5.2.s5"></a>File URL
文件URL旨在提供可从中接收附件的位置。然而，附件的所有者无法无限期地在该位置提供附件数据，或者使附件在没有安全限制的情况下公开可用。在确定附件托管安排时，鼓励使用“fileUrl”属性创建语句的那些人考虑该语句的最终收件人的需求，尤其是如果附件内容未包含在语句中

* <a name="1.5.2.s5.b1"></a>附件数据应该可以在fileUrl指示的URL处检索。
* <a name="1.5.2.s5.b2"></a>附件的所有者可以随时停止在此IRL提供附件数据。
* <a name="1.5.2.s5.b3"></a>安全限制可以对尝试访问此IRL中的附件数据的用户进行设置。

附件的可用时间段以及应用于托管附件的安全限制超出了本规范的范围。

###### <a name="1.5.2.s6"></a>Example

下面是一个带有附件的非常简单的Statement的例子。请注意以下事项：

* <a name="1.5.2.s6.b1"></a>选择样本中的边界是用来以证明有效的字符类
* <a name="1.5.2.s6.b2"></a>所选择的边界字符不作为任何内容的部分;
* <a name="1.5.2.s6.b3"></a>为了可读性，样本附件是“text / plain”类型。即使它是一个二进制类型，如“image / jpeg”，不进行编码，原始的八位字节将被包括;
* <a name="1.5.2.s6.b4"></a>根据RFC 2046，边界是`<CRLF>`（换行符）后面跟着 –再跟着 在header中声明的边界字符串。


__Note:__ Don't forget the ```<CRLF>```  when building or parsing these messages. 当构建消息时别忘了换行符`<CRLF>`
Headers:

``` 
Content-Type: multipart/mixed; boundary="abcABC0123'()+_,-./:=?"
X-Experience-API-Version:1.0.0
```
Content:
```

--abcABC0123'()+_,-./:=?
Content-Type:application/json

{
    "actor": {
        "mbox": "mailto:sample.agent@example.com",
        "name": "Sample Agent",
        "objectType": "Agent"
    },
    "verb": {
        "id": "http://adlnet.gov/expapi/verbs/answered",
        "display": {
            "en-US": "answered"
        }
    },
    "object": {
        "id": "http://www.example.com/tincan/activities/multipart",
        "objectType": "Activity",
        "definition": {
            "name": {
                "en-US": "Multi Part Activity"
            },
            "description": {
                "en-US": "Multi Part Activity Description"
            }
        }
    },
    "attachments": [
        {
            "usageType": "http://example.com/attachment-usage/test",
            "display": { "en-US": "A test attachment" },
            "description": { "en-US": "A test attachment (description)" },
            "contentType": "text/plain; charset=ascii",
            "length": 27,
            "sha2": "495395e777cd98da653df9615d09c0fd6bb2f8d4788394cd53c56a3bfdcd848a"
        }
    ]
}
--abcABC0123'()+_,-./:=?
Content-Type:text/plain
Content-Transfer-Encoding:binary
X-Experience-API-Hash:495395e777cd98da653df9615d09c0fd6bb2f8d4788394cd53c56a3bfdcd848a

here is a simple attachment
--abcABC0123'()+_,-./:=?--
```

<a name="datatransfer"/> <a name="resources"/>
## <a name="2.0">2.0</a> Resources 资源
LRS通过RESTful HTTP方法与本节中介绍的资源进行交互。语句资源本身可用于跟踪学习记录。其他资源提供了附加功能。

LRS将支持本节中描述的所有资源。不是LRS的工具也可以是选择遵循本节中描述的一个或多个资源和方法的LRS要求。例如，工具可能会实施POST语句，以接收由LRS转发的入局语句。这样的系统不被认为是LRS或“部分LRS”;但它不是一个LRS。

__Note:__ 在规范中给定xAPI资源所在的所有示例端点中，http://example.com/xAPI/是LRS的示例基本端点。此后的所有其他IRI语法表示所使用的特定资源。完整的端点列表包含在附录B：所有资源表中。 [Appendix B: Table of All Resources](#Appendix3B).

###### <a name="2.0.s1"></a>Requirements

* <a name="2.0.s1.b1"></a>LRS必须支持本节中描述的所有资源。
* <a name="2.0.s1.b2"></a>如果LRS实现OAuth 1.0，LRS还必须支持OAuth授权范围中描述的所有OAuth资源。 [OAuth Authorization Scope](#oauthscope).
* <a name="2.0.s1.b3"></a>LRS可能支持本规范中未描述的其他资源。
* <a name="2.0.s1.b4"></a>本规范的过去，当前和未来版本没有也不会定义具有以`extensions/`开头的路径段的端点。支持在本规范中未定义的附加资源的LRS应当定义它们的端点，其路径段以`extensions/` .

<a name="stmtres"/> 

#### <a name="2.1">2.1</a> Statement Resource 语句资源
###### <a name="2.1.s1"></a>Description 描述
xAPI的基本通信机制

<a name="stmtresput"/>

#### <a name="2.1.1">2.1.1</a> PUT Statements PUT 语句
###### <a name="2.1.1.s1"></a>Details 详情
Example endpoint 示例终端: `http://example.com/xAPI/statements` 


Stores a single Statement with the given id. POST can also be used to store single Statements.
储存一个单独的语句，POST也能实现

**Content内容:** The Statement object to be stored.  将要被储存的语句

**Returns返回值:** `204 No Content`  
<table>
	<tr><th>Parameter</th><th>Type</th><th>Default</th><th>Description</th><th>Required</th></tr>
	<tr id="2.1.1.s1.table1.row1"><td>statementId</td><td>String</td><td> 
	<td>Id of Statement to record<br>被储存语句的ID</td></td><td>Required</td></tr>
</table>

###### <a name="2.1.1.s2"></a>LRS Requirements 对LRS的要求
* <a name="2.1.1.s2.b1"></a>LRS可以在已存储的语句可用于检索之前进行响应。

* <a name="2.1.1.s2.b2"></a>对于接受的有着已经储存了的语句ID的语句，LRS不得对其状态进行修改，无论它响应`409 Conflict`还是`204 No Content`，它不得修改语句或任何其他对象。

* <a name="2.1.1.s2.b3"></a>如果LRS接收到一个带有ID的语句，它已经有一个语句，它应该验证接收的语句匹配现有的语句，如果它们不匹配应该返回 `409 Conflict` 。请参阅语句比较要求 [Statement comparison requirements](./xAPI-Data.md#statement-comparison-requirements).

* <a name="2.1.1.s2.b4"></a>如果LRS收到包含两个或多个具有相同ID的语句的一批语句，则它应该拒绝该批处理并返回 `400 Bad Request`.



###### <a name="2.1.1.s3"></a>Learning Record Provider Requirements 对LRP的要求

* <a name="2.1.1.s3.b1"></a>学习记录提供者应该POST语句，包括语句“id”属性，而不是使用PUT
* <a name="2.1.1.s3.b2"></a>当PUTing语句时，应该使用语句的“id”属性。
* <a name="2.1.1.s3.b3"></a>如果提供，语句的“id”属性必须匹配请求的“statementId”参数。

<a name="stmtrespost"/>

#### <a name="2.1.2">2.1.2</a> POST Statements POST语句

###### <a name="2.1.2.s1"></a>Details详情

Example endpoint 示例终端: `http://example.com/xAPI/statements`

Stores a Statement, or a set of Statements. 储存一个语句，或者设置一个语句

**Content内容:** An array of Statements or a single Statement to be stored.  一组要被储存的语句或一个语句

**Returns返回值:** `200 OK`, Array of Statement id(s) (UUID) in the same order as the corresponding stored Statements（和储存顺序一样顺序的语句UUID的数组）.  

###### <a name="2.1.2.s2"></a>Requirements 要求
* <a name="2.1.2.s2.b1"></a>LRS可以在已存储的语句可用于检索之前进行响应。
* <a name="2.1.2.s2.b2"></a>GET语句可以使用POST和表单参数调用，如果有必要，因为查询字符串有限制。有关详细信息，请参阅备用请求语法。 [Alternate Request Syntax](#alt-request-syntax)
* <a name="2.1.2.s2.b3"></a>LRS必须区分POST以添加语句或列出基于传递的参数的语句。有关详细信息，请参阅备用请求语法。 [Alternate Request Syntax](#alt-request-syntax) 
* <a name="2.1.2.s2.b4"></a>LRS不得对其状态进行任何修改，基于接收具有已经具有语句的ID的语句。无论它响应`409 Conflict`还是`204 No Content`，它不得修改语句或任何其他对象。 
* <a name="2.1.2.s2.b5"></a>如果LRS接收到一个带有ID的语句，它已经有一个语句，它应该验证接收的语句匹配现有的语句，如果它们不匹配应该返回`409 Conflict`。请参阅语句比较要求。 [Statement comparison requirements](./xAPI-Data.md#statement-comparison-requirements).
* <a name="2.1.2.s2.b6"></a>如果LRS收到包含两个或多个具有相同ID的语句的一批语句，则它应该拒绝该批处理并返回 `400 Bad Request`.

<a name="stmtresget"/>

#### <a name="2.1.3">2.1.3</a> GET Statements GET 语句

###### <a name="2.1.3.s1"></a>Details 详情

Example endpoint示例终端: `http://example.com/xAPI/statements`

调用此方法以获取单个语句或多个语句。如果指定statementId或voidedStatementId参数，则返回单个语句。

否则返回：[StatementResult](./xAPI-Data.md#retrieval)对象，基于"stored"时间的反向时间顺序的语句列表，受限于权限和最大列表长度。如果有其他结果可用，那么检索它们的IRL将包含在StatementResult对象中

**Content内容:** None.

**Returns返回值:** `200 OK`, Statement or [Statement Result](./xAPI-Data.md#retrieval)

<table>
	<tr><th>Parameter</th><th>Type</th><th>Default</th><th>Description</th><th>Required</th></tr>
	<tr id="2.1.3.s1.table1.row1">
		<td>statementId</td>
		<td>String</td>
		<td> </td>
		<td>Id of Statement to fetch<br>要获取的语句ID</td>
		<td>Optional</td>
	</tr>
	<tr id="2.1.3.s1.table1.row2">
		<td>voidedStatementId</td>
		<td>String</td>
		<td> </td>
		<td>Id of voided Statement to fetch.<br>要被无效化的语句的ID 见 <a href="./xAPI-Data.md#voided">Voided
		Statements</a></td>
		<td>Optional</td>
	</tr>
	<tr id="2.1.3.s1.table1.row3">
		<td>agent</td>
		<td>Agent or Identified Group Object (JSON)</td>
		<td> </td>
		<td>Filter, only return Statements for which the specified Agent or Group is 
		the Actor or Object of the Statement.<br>筛选器，只返回指定的代理或者组作为语句Actor或者Object的语句
			<ul>
				<li> 
					Agents or Identified Groups are equal when the same 
					Inverse Functional Identifier is used in each Object compared and 
					those Inverse Functional Identifiers have equal values.<br>
					当在比较的每个对象中使用相同的反函数标识符并且那些反函数标识符具有相等的值时，代理或识别的组是相等的。
				</li><li>
					For the purposes of this filter, Groups that have members 
					which match the specified Agent	based on their Inverse Functional
					Identifier as described above are considered a match<br>
					为了该过滤器的目的，具有基于如上所述的其反函数标识符匹配指定代理的成员的组被认为是匹配
</li>
			</ul>
			<br><br>参阅 <a href="./xAPI-Data.md#actor">agent/group</a> 对象的定义
		</td>
		<td>Optional</td>
	</tr>
	<tr id="2.1.3.s1.table1.row4">
		<td>verb</td>
		<td>Verb id (IRI)</td>
		<td> </td>
		<td>Filter, only return Statements matching the specified Verb id.<br>筛选器，只返回特定Verb的语句</td>
		<td>Optional</td>
	</tr>
	<tr id="2.1.3.s1.table1.row5">
		<td>activity</td>
		<td>Activity id (IRI)</td>
		<td> </td>
		<td>
			Filter, only return Statements for which the Object of the Statement is 
			an Activity with the specified id.<br>
			筛选器，只返回特定活动的语句
		</td>
		<td>Optional</td>
	</tr>
	<tr id="2.1.3.s1.table1.row6">
		<td>registration</td>
		<td>UUID</td>
		<td> </td>
		<td>
			Filter, only return Statements matching the specified registration 
			id. Note that although frequently a unique registration will be used 
			for one Actor assigned to one Activity, this cannot be assumed. 
			If only Statements for a certain Actor or Activity are required, 
			those parameters also need to be specified.<br>
			筛选器，只返回与指定的注册ID匹配的语句。请注意，尽管频繁地将唯一注册用于分配给一个活动的一个活动，但不能假定。如果只需要某个Actor或Activity的语句，则还需要指定这些参数。
		</td>
		<td>Optional</td>
	</tr>
	<tr id="2.1.3.s1.table1.row7">
	<td>related_activities</td>
		<td>Boolean</td>
		<td>false</td>
		<td>
			Apply the Activity filter broadly. Include Statements for which the Object,
			any of the  context Activities, or any of those properties in a contained
			SubStatement match the Activity parameter, instead of that parameter's 
			normal behavior. Matching is defined in the same way it is for the 
			"activity" parameter.<br>广泛应用活动过滤器。包括对象，任何上下文活动或所包含的SubStatement中的任何属性与“活动”参数匹配的语句，而不是该参数的正常行为。匹配以与“活动”参数相同的方式定义。
</td>
		<td>Optional</td>
	</tr>
	<tr id="2.1.3.s1.table1.row8">
		<td>related_agents</td>
		<td>Boolean</td>
		<td>false</td>
		<td>
			Apply the Agent filter broadly. Include Statements for which 
			the Actor, Object, Authority, Instructor, Team,
			or any of these properties in a contained SubStatement match the Agent parameter,
			instead of that parameter's normal behavior. Matching is defined in the same way
			it is for the "agent" parameter.<br>广泛应用代理过滤器。包含所包含的SubStatement中的Actor，Object，Authority，Instructor，Team或任何这些属性与代理参数匹配的语句，而不是该参数的正常行为。匹配以与“代理”参数相同的方式定义。
		</td>
		<td>Optional</td>
	</tr>
	<tr id="2.1.3.s1.table1.row9">
		<td>since</td>
		<td>Timestamp</td>
		<td> </td>
		<td>Only Statements stored since the specified Timestamp (exclusive) are returned.<br>只返回自此之后的语句</td>
		<td>Optional</td>
	</tr>
	<tr id="2.1.3.s1.table1.row10">
		<td>until</td>
		<td>Timestamp</td>
		<td> </td>
		<td>Only Statements stored at or before the specified Timestamp are returned.<br>只返回自此之前的语句</td>
		<td>Optional</td>
	</tr>
	<tr id="2.1.3.s1.table1.row11">
		<td>limit</td>
		<td>Nonnegative Integer</td>
		<td>0</td>
		<td>
			Maximum number of Statements to return. 0 indicates return the 
			maximum the server will allow.<br>返回的最大语句数量的限制
</td>
		<td>Optional</td>
	</tr>
	<tr id="2.1.3.s1.table1.row12">
		<td>format</td>
		<td>String: (<code>ids</code>, <code>exact</code>, or <code>canonical</code>)</td>
		<td>exact</td>
		<td>If <code>ids</code>, only include minimum information necessary in Agent, Activity, Verb 
			and Group Objects to identify them. For Anonymous Groups this means including 
			the minimum information needed to identify each member. 
			<br/><br/>
			如果为<code>ids</code>，只包括代理，活动，动词和组对象中必要的最小信息，以识别它们。对于匿名组，这意味着包括识别每个成员所需的最少信息。<br/><br/>
			
			If <code>exact</code>, return Agent, Activity, Verb and Group Objects populated exactly as they 
			were when the Statement was received. An LRS requesting Statements for the purpose 
			of importing them would use a format of "exact" in order to maintain 
			<a href="./xAPI-Data.md#statement-immutability-and-exceptions">Statement Immutability</a>.  
			<br/><br/>
			如果为<code>exact</code>，返回代理，活动，动词和组对象填充完全一样，当收到语句时。 LRS要求声明用于导入它们将使用"exact"的格式，以维持声明不可变性。
			<br/><br/>
			If <code>canonical</code>, return Activity Objects and Verbs populated with the canonical
			definition of the Activity Objects and Display of the Verbs as determined by the LRS, after
			applying the <a href="#queryLangFiltering">language filtering process defined below</a>,
			and return the original Agent and Group Objects as in "exact" mode.  
			<br/><br/>
			如果是<code>canonical</code>，则在应用以下定义的语言过滤过程后，返回填充有由LRS确定的活动对象和动词的显示的规范定义的活动对象和动词，并以"exact"模式返回原始“Agent和Group对象”。
		</td>
		<td>Optional</td>
	</tr>
	<tr id="2.1.3.s1.table1.row13">
		<td>attachments</td><td>Boolean</td><td>false</td>
		<td>If <code>true</code>, the LRS uses the multipart response format and includes all attachments as 
		described previously.<br/>如果为<code>true</code>，则LRS使用多部分响应格式，并包括如前所述的所有附件。<br>  If <code>false</code>, the LRS sends the prescribed response with Content-Type 
		application/json and does not send attachment data.<br>如果为<code>false</code>，则LRS使用Content-Type为 application / json发送规定的响应，并且不发送附件数据。</td>
		<td>Optional</td>
	</tr>
	<tr id="2.1.3.s1.table1.row14">
		<td>ascending</td>
		<td>Boolean</td>
		<td>false</td>
		<td>If <code>true</code>, return results in ascending order of stored time<br/>如果为<code>true</code>，则按存储时间的升序返回结果</td>
		<td>Optional</td>
	</tr>
</table>

__Note:__ 布尔参数的值在JSON中表示为`true` or `false` 
###### <a name="2.1.3.s2"></a>Requirements

* <a name="2.1.3.s2.b1"></a>LRS务必以`400 Bad Request`拒绝任何同时包含statementId和voidedStatementId参数的请求资源

* <a name="2.1.3.s2.b2"></a>LRS务必以`400 Bad Request`拒绝任何包含了statementId或者voidedStatementId参数并且又包含除了‘attachments’和‘format’之外参数的请求资源

* <a name="2.1.3.s2.b3"></a>LRS可以基于与所使用的凭证相关联的权限来应用附加的查询过滤器条件。

* <a name="2.1.3.s2.b4"></a>如果没有找到与查询过滤器条件匹配的语句，则LRS必须仍然返回`200 OK`和[StatementResult](./xAPI-Data.md#retrieval)对象。在这种情况下，“statements”属性将包含一个空数组。 

* <a name="2.1.3.s2.b5"></a>LRS必须在对于语句资源请求的所有响应上包括以[ISO 8601 combined date and time](https://en.wikipedia.org/wiki/ISO_8601#Combined_date_and_time_representations)格式的标题“X-Experience-API-Consistent-Through”，其中所有具有或将要有的语句的时间戳的值在该时间之前的“stored”属性已知具有可用于检索的合理确定性。这个时间应该考虑任何临时情况，例如过度负载，这可能导致语句的延迟变得可用于检索。预计这将是最近的时间戳，即使没有最近收到的语句。

* <a name="2.1.3.s2.b6"></a>如果使用GET语句的“附件”属性并设置为true，则LRS必须使用多部分响应格式，并包括第二部分 [Part Two](./xAPI-Data.md#attachments).中所述的所有附件。

* <a name="2.1.3.s2.b7"></a>如果使用GET语句的“Attachment”属性并设置为`false`，则LRS不得包括附件原始数据，并且必须返回 `application/json`

* <a name="2.1.3.s2.b8"></a>LRS应该包括一个"Last-Modified"头，它匹配语句的“存储”时间戳。

<a name="queryStatementRef" />

###### <a name="2.1.3.s3"></a>Filter Conditions for StatementRefs StatementRef的过滤条件

本部分概述了定位其他语句的语句有时可以被视为满足查询的过滤条件，即使它们与原始查询的过滤器参数不匹配的规则。当使用“statementId”或“voidedStatementId”查询参数检索单个语句时，这些规则不适用。

'Targeting Statements''定向语句'意味着一个语句（目标语句）包括另一个语句（目标语句）的语句id作为语句对象的语句引用

对于不是基于时间或序列（即除了“since”，“until”或“limit”之外）的过滤器参数，以其他语句为目标的语句（通过使用StatementRef作为语句的对象）将满足过滤条件（如果目标语句满足过滤条件）

基于时间和基于序列的参数必须仍然应用于语句，使StatementRef以这种方式。该规则递归地应用，这就意味着“语句a”将会找到“语句c”，当语句a定向b而b又定向c时。

例如：一个语句“本通过了爆炸训练”，和另外一个语句“阿黛尔审核了该结果” 当检索时候如果检索时间点刚好在两个语句的时间之间，那么是会将两个语句都返回的，而不是只返回检索时间点之前或者之后的那个。

__Note:__ 用作上下文中“语句”属性的值的StatementRef不会影响语句的过滤方式

<a name="queryLangFiltering" />

###### <a name="2.1.3.s4"></a>Language Filtering Requirements for Canonical Format Statements 规范格式语句的语言过滤要求

* <a name="2.1.3.s4.b1"></a>活动对象在其“名称”，“描述”和各种交互组件中包含语言映射对象。 LRS必须在每个映射中只返回一种语言。

* <a name="2.1.3.s4.b2"></a>LRS可以针对任何IRI识别包含语言映射的对象来保持语言映射的规范版本。这包括存储在动词的“display”属性中的语言映射，以及扩展中使用的一些语言映射。 

* <a name="2.1.3.s4.b3"></a>如果LRS维护语言映射的规范版本，那么当规范格式用于检索语句时，它应该返回这个规范语言映射。

* <a name="2.1.3.s4.b4"></a>LRS SHOULD *在每个语言映射中只返回一种语言，它返回一个规范映射。

* <a name="2.1.3.s4.b5"></a>为了选择最相关的语言，LRS必须应用[RFC 2616](http://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html)中描述的“Accept-Language”报头，除了该逻辑务必单独应用于每个语言映射以选择要包括哪个语言条目，而不是整个资源（报表清单）。 
<a name="voidedStatements" />

##### <a name="2.1.4">2.1.4</a> Voided Statements 无效化语句
[Part Two](./xAPI-Data.md#voided) 第二部分--描述了可以废除语句的过程。本节描述了查询时LRS处理无效语句的方式。

客户可以通过无效声明的目标来识别任何已失效声明的存在和声明ID。除了调试工具外，许多学习记录消费者不希望向其用户显示无效语句，并且不会将它们显示为活动流和其他报告的一部分。

###### <a name="2.1.4.s1"></a>Requirements

* <a name="2.1.4.s1.b1"></a>LRS不得返回任何已被废除的语句，除非该语句已由voidedStatementId请求。在StatementRefs的过滤条件[the section on filter conditions for StatementRefs](#queryStatementRef) 一节中描述的过程也不是这个要求的例外。检索voiding语句的过程是通过voidedStatementId单独请求每个。 
* <a name="2.1.4.s1.b2"></a>LRS还必须按照StatementRefs的过滤条件部分[the section on filter conditions for StatementRefs](#queryStatementRef)中描述的过程和条件，返回任何以无效语句为目标的语句。这包括voiding Statement，它不能被无效。
<a name="doctransfer"/>

### <a name="2.2">2.2</a> Document Resources  文档资源

##### <a name="2.2.s1"></a>Description 描述
体验API为学习记录提供者提供了一种设施，以文档的形式保存任意数据，可能与活动，代理或两者的组合相关。

##### <a name="2.2.s2"></a>Details 详情
请注意，下表显示了通用属性，而不是本规范中许多其他表中的JSON对象。 id存储在IRL中，“updated”是HTTP头信息，“contents”是HTTP文档本身（与Object不同）。
<table>
	<tr><th>Property</th><th>Type</th><th>Description</th></tr>
	<tr id="2.2.s2.table1.row1"><td>id</td><td>String</td><td>Set by Learning Record Provider, unique within the scope 
	of the Agent or Activity.<br>由学习记录提供者设置，在代理或活动的范围内是唯一的。</td></tr>
	<tr id="2.2.s2.table1.row2"><td>updated</td><td>Timestamp</td><td>When the document was most recently modified.<br>最近的文档修改时间。</td></tr>
	<tr id="2.2.s2.table1.row3"><td>contents</td><td>Arbitrary binary data</td><td>The contents of the document<br>文档的内容</td></tr>
</table>

三个文档资源[document](./xAPI-Data.md#documents)提供文档存储。每个资源的详细信息在以下部分中找到，本节中的信息适用于所有三个资源。 

###### <a name="2.2.s3"></a>Details 详情
<table>
	<tr>
		<th>Resource</th>
		<th>Method</th>
		<th>Endpoint</th>
		<th>Example</th>
	</tr>
	<tr id="2.2.s3.table1.row1">
		<td>State Resource</td>
		<td>POST</td>
		<td>activities/state</td>
		<td>http://example.com/xAPI/activities/state</td>
	</tr>
	<tr id="2.2.s3.table1.row2">
		<td>Activity Profile Resource</td>
		<td>POST</td>
		<td>activities/profile</td>
		<td>http://example.com/xAPI/activities/profile</td>
	</tr>
	<tr id="2.2.s3.table1.row3">
		<td>Agent Profile Resource</td>
		<td>POST</td>
		<td>agents/profile</td>
		<td>http://example.com/xAPI/agents/profile</td>
	</tr>
</table>

###### <a name="2.2.s4"></a>Requirements

* <a name="2.2.s4.b1"></a>学习记录提供者可以将文档发送到LRS没有先前知识的任何活动和代理的文档资源。

* <a name="2.2.s4.b2"></a>LRS不得基于不具有活动和/或代理的先验知识而拒绝文档。

##### <a name="2.2.s5"></a>Last Modified
 当返回单个或多个文档以响应GET请求时，"Last Modified"标题由LRS设置。

###### <a name="2.2.s6"></a>Requirements
* <a name="2.2.s6.b1"></a>当返回单个文档时，LRS应该*包括一个“Last-Modified”标题，指示文档上次修改的时间
* <a name="2.2.s6.b2"></a>当返回多个文档时，LRS应该包括“Last-Modified”标题，指示最近修改的文档何时被最后修改。

###### <a name="2.2.s7"></a>JSON Procedure with Requirements JSON过程与需求

如果学习记录提供者将变量作为JSON对象存储在内容类型为`application/json`的文档中，他们可以使用POST将它们作为一组变量操作。

以下过程将介绍该过程和过程要求。
例如，文档包含： 

```
{
	"x" : "foo",
	"y" : "bar"
}
```  
当LRS接收到对内容类型为`application/json`的现有文档的内容类型也为`application/json`的POST请求时，它必须合并所发布的文档与现有文档。在此上下文中，合并被定义为：
* <a name="2.2.s7.b1"></a>对每个文档表示的对象解序列化
* <a name="2.2.s7.b2"></a>对于在正在发布的对象上直接定义的每个属性，将现有对象上的相应属性设置为等于发布对象的值。   
* <a name="2.2.s7.b3"></a>存储现有对象的任何有效的json序列化作为请求中引用的文档。

注意，只有顶级属性被合并，即使顶级属性是一个对象。每个原始属性的全部内容将替换为每个新属性的全部内容
例如，此文档使用与上述现有文档相同的ID进行POST：
```
{
	"x" : "bash",
	"z" : "faz"
}
```  
存储在LRS中的结果文档是：
```
{
	"x" : "bash",
	"y" : "bar",
	"z" : "faz"
}
```

###### <a name="2.2.s8"></a>Requirements

* <a name="2.2.s8.b1"></a>如果正在发布的文档或任何现有文档没有`application/json`的Content-Type，或者任何一个文档不能解析为JSON对象，则LRS务必使用HTTP状态代码`400 Bad Request`请求，并且不得更新目标文档作为请求的结果

* <a name="2.2.s8.b2"></a>如果合并成功，则LRS务必使用HTTP状态代码 `204 No Content`进行响应。

* <a name="2.2.s8.b3"></a>如果学习记录提供者需要删除属性，它应该使用PUT请求来替换整个文档，如下所述。 

<a name="stateres"/> 

### <a name="2.3">2.3</a> State Resource 状态资源
##### <a name="2.3.s1"></a>Description 描述
通常，这是学习记录提供程序的划痕区域，它没有自己的内部存储器，或者需要跨设备保持状态。

##### <a name="2.3.s2"></a>Details

调用的语义由“stateId”参数驱动。而GET和DELETE方法将作用于由“stateId”标识的单个定义的状态文档，如果包括的话。否则，GET将返回可用的ID，DELETE将删除通过其他参数给定的上下文中的所有状态。此资源具有与其相关联的并发[Concurrency](#concurrency)控件。


###### <a name="2.3.s3"></a>Single Document (PUT | POST | GET | DELETE) 单个文档（PUT,POST,GET,DELETE）

Example endpoint示例终端: http://example.com/xAPI/activities/state

存储，更改，删除或删除由指定的Activity，代理和注册（如果指定）的上下文中存在的给定“stateId”指定的文档 

**Content (PUT | POST):** The document to be stored or updated. 要被更新或储存的文档  
**Content (GET | DELETE):** None.  

**Returns (PUT | POST | DELETE):** `204 No Content`  
**Returns (GET):** `200 OK`, the State document 
<table>
	<tr><th>Parameter</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.3.s3.table1.row1">
		<td>activityId</td>
		<td>Activity id (IRI)</td>
		<td>The Activity id associated with this state.<br>与此状态相关联的活动ID</td>
		<td>Required</td>
	</tr>
	<tr id="2.3.s3.table1.row2">
		<td>agent</td>
		<td>Agent Object (JSON)</td>
		<td>The Agent associated with this state.<br>与此状态相关联的代理</td>
		<td>Required</td>
	</tr>
	<tr id="2.3.s3.table1.row3">
		<td>registration</td>
		<td>UUID</td>
		<td>The registration associated with this state.<br>与此状态相关联的注册</td>
		<td>Optional</td>
	</tr>
	<tr id="2.3.s3.table1.row4">
		<td>stateId</td>
		<td>String</td>
		<td>The id for this state, within the given context<br>有着相应内容的状态id</td>
		<td>Required</td>
	</tr>
</table>

###### <a name="2.3.s4"></a>Multiple Document GET 多文档GET

Example endpoint 示例终端: http://example.com/xAPI/activities/state

获取此上下文的所有状态数据的状态ID（活动+代理[如果指定，则为+注册]）。如果指定“since”参数，则仅限于自指定时间戳（独占）以来已存储或更新的条目。

**Content:** None.

**Returns:** `200 OK`, Array of State id(s)  

<table>
	<tr><th>Parameter</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.3.s4.table1.row1">
		<td>activityId</td>
		<td>Activity id (IRI)</td>
		<td>The Activity id associated with these states.<br>与此状态相关联的活动ID</td>
		<td>Required</td>
	</tr>
	<tr id="2.3.s4.table1.row2">
		<td>agent</td>
		<td>Agent object (JSON)</td>
		<td>The Agent associated with these states.<br>与此状态相关联的代理</td>
		<td>Required</td>
	</tr>
	<tr id="2.3.s4.table1.row3">
		<td>registration</td>
		<td>UUID</td>
		<td>The Registration associated with these states.<br>与此状态相关联的注册</td>
		<td>Optional</td>
	</tr>
	<tr id="2.3.s4.table1.row4">
		<td>since</td>
		<td>Timestamp</td>
		<td>Only ids of states stored since the specified Timestamp (exclusive) are returned.<br>只返回指定的时间戳（独占）后存储的状态的ID。</td>
		<td>Optional</td>
	</tr>
</table>

###### <a name="2.3.s5"></a>Multiple Document DELETE 多文档删除

Example endpoint 示例终端: http://example.com/xAPI/activities/state

删除此上下文的所有状态数据（Activity + Agent [+注册（如果指定）]）.  

**Content:** None.

**Returns**: `204 No Content`  
<table>
	<tr><th>Parameter</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.3.s5.table1.row1">
		<td>activityId</td>
		<td>Activity id (IRI)</td>
		<td>The Activity id associated with this state.<br>与此状态相关联的活动ID</td>
		<td>Required</td>
	</tr>
	<tr id="2.3.s5.table1.row2">
		<td>agent</td>
		<td>Agent object (JSON)</td>
		<td>The Agent associated with this state.<br>与此状态相关联的代理</td>
		<td>Required</td>
	</tr>
	<tr id="2.3.s5.table1.row3">
		<td>registration</td>
		<td>UUID</td>
		<td>The Registration associated with this state.<br>与此状态相关联的注册</td>
		<td>Optional</td>
	</tr>
</table>

<a name="agentsres"/>

### <a name="2.4">2.4</a> Agents Resource

代理资源提供了一种检索特殊对象的方法，该对象具有关于从外部服务（如目录服务）派生的代理的组合信息。此资源具有与其相关联的并发[Concurrency](#concurrency)控件。 

###### <a name="2.4.s1"></a>Combined Information GET 组合信息GET

###### <a name="2.4.s2"></a>Details 详情

Example endpoint 示例终端: http://example.com/xAPI/agents

返回指定代理的特殊Person对象。 Person对象与代理对象非常相似，但每个属性具有单个值，而不是每个属性具有一个数组值，并且包含多个标识属性是合法的。这不同于人的FOAF概念，人在这里被用来表示LRS代理数据的以人为中心的视图，但是代理只是指一个人物（在一个上下文中的人）。 

“代理”参数是具有单个标识符且没有数组的正常代理对象。它不是一个Person对象，也不是一个Group。
**Content:** None.

**Returns:** `200 OK`, Person Object

<table>
	<tr><th>Parameter</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.4.s2.table1.row1">
		<td>agent</td>
		<td>Agent object (JSON)</td>
		<td>The Agent representation to use in fetching expanded Agent information.<br>用于获取扩展代理信息的代理表示。</td>
		<td>Required</td>
	</tr>
</table>

###### <a name="2.4.s3"></a>Requirements
* <a name="2.4.s3.b1"></a>能够返回Person对象的多个标识属性的LRS应该要求连接凭证增加了明确给定的权限。
* <a name="2.4.s3.b2"></a>LRS应该使用 `403 Forbidden`拒绝不够特权的请求。
* <a name="2.4.s3.b3"></a>如果LRS没有关于要返回的代理的任何附加信息，则LRS必须在查询时仍返回Person对象，但该Person对象将仅包括与所请求的代理相关联的信息

__Note:__这意味着如果针对LRS没有预先知识的代理发出请求，它将仍然返回一个Person对象，其中包含有关在请求中收到的代理的信息。

###### <a name="2.4.s4"></a>Person Properties

###### <a name="2.4.s5"></a>Details

<table>
	<tr><th>Property</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.4.s5.table1.row1">
		<td>objectType</td>
		<td>String</td>
		<td><code>Person</code></td>
		<td>Required</td>
	</tr>
	<tr id="2.4.s5.table1.row2">
		<td>name</td>
		<td>Array of strings.</td>
		<td>List of names of Agents retrieved.<br>检索的代理的名称列表。</td>
		<td>Optional</td>
	</tr>
	<tr id="2.4.s5.table1.row3">
		<td><a href="http://xmlns.com/foaf/spec/#term_mbox">mbox</a></td>
		<td>Array of IRIs in the form "mailto:email address".</td>
		<td>List of e-mail addresses of Agents retrieved.<br>检索的代理的email列表</td>
		<td>Optional</td>
	</tr>
	<tr id="2.4.s5.table1.row4">
		<td><a href="http://xmlns.com/foaf/spec/#term_mbox_sha1sum">mbox_sha1sum</a></td>
		<td>Array of strings.</td>
		<td>List of the SHA1 hashes of mailto IRIs (such as go in an mbox property).<br>检索的代理的邮箱sha1哈希列表</td>
		<td>Optional</td>
	</tr>
	<tr id="2.4.s5.table1.row5">
		<td>openid*</td>
		<td>Array of strings.</td>
		<td>List of openids that uniquely identify the Agents retrieved.<br>唯一标识检索到的代理的openids列表</td>
		<td>Optional</td>
	</tr>
	<tr id="2.4.s5.table1.row6">
		<td>account*</td>
		<td>Array of account objects.</td>
		<td>List of accounts to match. Complete account Objects (homePage and name) 
		MUST be provided.<br>要匹配的帐户列表。必须提供完整的帐户对象（homePage和名称）。</td>
		<td>Optional</td>
	</tr>
</table>

可参见: [Agent](./xAPI-Data.md#agent).

###### <a name="2.4.s6"></a>Requirements

* <a name="2.4.s6.b1"></a>所有数组属性必须填充来自代理对象的类似命名的属性且具有相同定义的参数。 

* <a name="2.4.s6.b2"></a>此处未列出的附加属性SHOULD *不应添加到此对象，每个属性必须只发生一次。 

<a name="activitiesres"/> 

### <a name="2.5">2.5</a> Activities Resource 活动资源
The Activities Resource provides a method to retrieve a full description of an Activity from the LRS. 
This resource has活动资源提供了一种从LRS检索活动的完整描述的方法。此资源具有与其相关联的并发 [Concurrency](#concurrency)控件。

###### <a name="2.5.s1"></a>Full Activity Object GET 完整活动对象GET
Example endpoint示例终端: http://example.com/xAPI/activities

加载指定的完整活动对象。

**Content:** None.

**Returns:** `200 OK`, Content 
<table>
	<tr><th>Parameter</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.5.s1.table1.row1">
		<td>activityId</td>
		<td>Activity id (IRI)</td>
		<td>The id associated with the Activities to load.<br>与要加载的活动相关联的ID。</td>
		<td>Required</td>
	</tr>
</table>

###### <a name="2.5.s2"></a>Requirements

* <a name="2.5.s2.b1"></a>如果LRS没有要返回的Activity的规范定义，则LRS SHOULD *在查询时仍然返回活动对象。

<a name="agentprofres"/>

### <a name="2.6">2.6</a> Agent Profile Resource 代理配置资源

###### <a name="2.6.s1"></a>Description

代理配置文件资源非常类似于状态资源，允许保存与代理相关的任意密钥/文档对。

###### <a name="2.6.s2"></a>Details

请求的语义由“profileId”参数驱动。如果包括，GET方法将作用于由“profileId”标识的单个定义的文档。否则，GET将返回可用的ID。 

###### <a name="2.6.s3"></a>Single Agent or Profile Document (PUT | POST | GET | DELETE)

Example endpoint 示例终端: http://example.com/xAPI/agents/profile

在指定代理的上下文中存储，更改，获取或删除指定的Profile文档。

**Content (PUT | POST):** The document to be stored or updated.  
**Content (GET | DELETE):** None.  

**Returns (PUT | POST | DELETE):** `204 No Content`  
**Returns (GET):** `200 OK`, the Profile document  

<table>
	<tr><th>Parameter</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.6.s3.table1.row1">
		<td>agent</td>
		<td>Agent object (JSON)</td>
		<td>The Agent associated with this Profile document.<br>与此配置文件文档相关联的代理</td>
		<td>Required</td>
	</tr>
	<tr id="2.6.s3.table1.row2">
		<td>profileId</td>
		<td>String</td>
		<td>The profile id associated with this Profile document.<br>对应的配置文件id</td>
		<td>Required</td>
	</tr>
</table>

__Note:__ “代理”参数是代理对象，而不是组。学习记录希望针对已识别组存储数据的提供程序可以在代理对象中使用已识别组的标识符

###### <a name="2.6.s4"></a>Multiple Document GET 多文档GET

Example endpoint: http://example.com/xAPI/agents/profile

获取代理的所有配置文件文档的配置文件ID。如果指定了“since”参数，则仅限于自指定的时间戳（独占）以来已存储或更新的条目。

**Content:** None.

**Returns:** `200 OK`, Array of Profile id(s)  

<table>
	<tr><th>Parameter</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.6.s4.table1.row1">
		<td>agent</td>
		<td>Agent object (JSON)</td>
		<td>The Agent associated with this Profile document.<br>与此配置文件文档相关联的代理。</td>
		<td>Required</td>
	</tr>
	<tr id="2.6.s4.table1.row2">
		<td>since</td>
		<td>Timestamp</td>
		<td>Only ids of Profiles stored since the specified Timestamp 
			(exclusive) are returned.<br>想要返回的资源的上限时间点</td>
		<td>Optional</td>
	</tr>
</table>

<a name="actprofres"/> 

### <a name="2.7">2.7</a> Activity Profile Resource 活动配置资源
###### <a name="2.7.s1"></a>Description

活动配置文件资源非常类似于状态资源，允许保存与活动相关的任意密钥/文档对。

###### <a name="2.7.s2"></a>Details

请求的语义由“profileId”参数驱动。如果包括，GET方法将作用于由“profileId”标识的单个定义的文档。否则，GET将返回可用的ID。

###### <a name="2.7.s3"></a>Single Document (PUT | POST | GET | DELETE) 单独文档（PUT,POST,GET,DELETE）

Example endpoint 示例终端: http://example.com/xAPI/activities/profile

在指定的活动的上下文中存储，更改，获取或删除指定的Profile文档。

**Content (PUT | POST):** The document to be stored or updated.  
**Content (GET | DELETE):** None.  

**Returns (PUT | POST | DELETE)** `204 No Content`  
**Returns (GET):** `200 OK`, the Profile document  
<table>
	<tr><th>Parameter</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.7.s3.table1.row1">
		<td>activityId</td>
		<td>Activity id (IRI)</td>
		<td>The Activity id associated with this Profile document.<br>与此配置文件文档相关联的活动ID</td>
		<td>Required</td>
	</tr>
	<tr id="2.7.s3.table1.row2">
		<td>profileId</td>
		<td>String</td>
		<td>The profile id associated with this Profile document.<br>对应的配置文件id</td>
		<td>Required</td>
	</tr>
</table>
 
###### <a name="2.7.s4"></a>Multiple Document GET 多文档GET

Example endpoint 示例终端: http://example.com/xAPI/activities/profile

获取活动的所有配置文件文档的配置文件ID。如果指定了“since”参数，则仅限于自指定的时间戳（独占）以来已存储或更新的条目。

**Content:** None.

**Returns:** `200 OK`, Array of Profile id(s)  

<table>
	<tr id="2.7.s4.table1.row1"><th>Parameter</th><th>Type</th><th>Description</th><th>Required</th><tr>
	<tr>
		<td>activityId</td>
		<td>Activity id (IRI)</td>
		<td>The Activity id associated with these Profile documents.<br>与此配置文件文档相关联的活动id</td>
		<td>Required</td>
	</tr>
	<tr id="2.7.s4.table1.row2">
		<td>since</td>
		<td>Timestamp</td>
		<td>Only ids of Profile documents stored since the specified Timestamp (exclusive) 
		are returned.<br>想要返回的资源的上限时间点</td>
		<td>Optional</td>
	</tr>
</table>


<a name="aboutresource"/> 

### <a name="2.8">2.8</a> About Resource  About资源

###### <a name="2.8.s1"></a>Description 

返回包含有关此LRS的信息的JSON对象，包括受支持的xAPI版本。

###### <a name="2.8.s2"></a>Rationale

主要是存在此资源，以允许支持多个xAPI版本的客户端决定在与LRS通信时使用哪个版本。包括扩展以允许其他用途出现。

###### <a name="2.8.s3"></a>Details

###### <a name="2.8.s4"></a>Information GET

Example endpoint: http://example.com/xAPI/about

**Content:** None.

**Returns:** `200 OK`, JSON object containing basic metadata about this LRS（包含着最基本的关于LRS的元数据的JSON对象）
<table border="1">
	<tr><th>Property</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.8.s4.table1.row1">
		<td>version</td>
		<td>Array of version strings</td>
		<td>xAPI versions this LRS supports<br>xAPI的版本</td>
		<td>Required</td>
	</tr>
	<tr id="2.8.s4.table1.row2">
		<td>extensions</td>
		<td><a href="./xAPI-Data.md#miscext">Object</a></td>
		<td>A map of other properties as needed<br>一系列的如需的属性</td>
		<td>Optional</td>
	</tr>

</table>

###### <a name="2.8.s5"></a>Requirements

* <a name="2.8.s5.b1"></a>LRS务必返回上面描述的JSON文档，每个主要版本都带有一个“version”属性，其中包含LRS所遵循的最新版本和补丁版本
    * <a name="2.8.s5.b1.b1"></a>对于本规范的`1.0.0`版本，这意味着必须包括`1.0.0`;`0.9`和`0.95`可以包括。 （出于本要求的目的，0.9和0.95被认为是主要版本。） 
* <a name="2.8.s5.b2"></a>其他属性不能添加到扩展之外的此对象，每个属性必须只发生一次。
* <a name="2.8.s5.b3"></a>LRS应该允许未经身份验证的访问此资源
* <a name="2.8.s5.b4"></a>LRS不得基于版本标头所要求的版本标头来拒绝请求。 [Versioning](#versioning).

<a name="validation"/> 

## <a name="3.0">3.0</a> Data Validation 数据验证

###### <a name="3.0.s1"></a>Description

xAPI中的LRS的功能是存储和检索语句。只要它具有足够的信息来执行这些任务，就可以期望它执行这些任务。xAPI中的语句的验证仅关注语法，而不是语义。在动词定义，活动类型和扩展中强制执行确保有效含义的规则是发送语句的学习记录提供者的责任。

###### <a name="3.0.s2"></a>Requirements

* <a name="3.0.s2.b1"></a>LRS应当执行关于结构的那些规则。
* <a name="3.0.s2.b2"></a>LRS不应执行有关意义的那些规则  

<a name="concurrency"/>

### <a name="3.1">3.1</a> Concurrency 并发

##### <a name="3.1.s1"></a>Description
并发控制确保客户端不会将基于旧数据的文档PUT，POST或DELETE文档放入LRS中。

##### <a name="3.1.s2"></a>Details
xAPI将使用HTTP 1.1实体标签 ([ETags](http://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html#sec14.19))在API的部分中实现乐观并发控制，其中PUT，POST或DELETE可能覆盖或删除现有数据，即：

* <a name="3.1.s2.b1"></a>State Resource 状态资源
* <a name="3.1.s2.b2"></a>Agent Profile Resource  代理配置资源
* <a name="3.1.s2.b3"></a>Activity Profile Resource 活动配置资源

##### <a name="3.1.s3"></a>Client Requirements
状态资源将允许没有并发头的PUT，POST和DELETE请求，因为状态冲突是不可能的。以下要求仅适用于座席配置文件资源和活动配置文件资源。

* <a name="3.1.s3.b1"></a>向代理配置文件资源或活动配置文件资源发出PUT请求的客户端必须包含 "[If-Match](http://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html#sec14.24)"头或[If-None-Match](http://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html#sec14.26)头。
* <a name="3.1.s3.b2"></a>向代理配置文件资源或活动配置文件资源发出POST请求的客户端必须包含 "[If-Match](http://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html#sec14.24)"头或[If-None-Match](http://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html#sec14.26)头。

* <a name="3.1.s3.b3"></a>向代理配置文件资源或活动配置文件资源发出DELETE请求的客户端应包含"[If-Match](http://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html#sec14.24)"头。

* <a name="3.1.s3.b4"></a>客户端应该使用由LRS提供的ETag值，而不是自己计算

##### <a name="3.1.s4"></a>LRS Requirements

* <a name="3.1.s4.b1"></a>响应GET请求的LRS必须向响应添加ETag HTTP头。
* <a name="3.1.s4.b2"></a>响应GET请求而不使用传输编码或使用身份传输编码的LRS必须计算ETag头的值为内容的SHA-1摘要的十六进制字符串。这个十六进制字符串应该只使用数字和小写字符来呈现;大写字符不应该使用。以此方式计算ETag的要求将在规范的未来版本中删除。
* <a name="3.1.s4.b3"></a>响应于使用任何非身份传输编码的GET请求的LRS不能如上所述计算所包括的ETag，这是由于现有web基础设施对ETag的解释
* <a name="3.1.s4.b4"></a>如[RFC 2616](http://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html#sec14.19)中定义的，响应GET请求的LRS必须将报头括在引号中。 
* <a name="3.1.s4.b5"></a>响应PUT请求的LRS必须处理如RFC2616，HTTP 1.1中所述的"[If-Match](http://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html#sec14.24)"报头（如果它包含ETag），以便检测客户端上次获取文档后所做的修改。 
* <a name="3.1.s4.b6"></a>响应于PUT请求的LRS必须处理如RFC2616，HTTP 1.1中所述的"[If-None-Match](http://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html#sec14.26)"报头，如果它包含“*”，以便检测何时存在客户端不知道的资源。 
* <a name="3.1.s4.b7"></a>响应POST或DELETE请求的LRS如果包含ETag，则处理如RFC2616（HTTP 1.1）中所述的"[If-Match](http://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html#sec14.24)"报头，以便检测客户端上次获取文档后所做的修改。 
* <a name="3.1.s4.b8"></a>响应于POST请求的LRS应处理如RFC2616，HTTP 1.1中所述的"[If-None-Match](http://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html#sec14.26)"报头，如果它包含“*”，以便检测何时存在客户端不知道的资源的。

如果上述任一PUT请求情况中的报头前提条件失败，则LRS：

* <a name="3.1.s4.b9"></a>必须返回HTTP状态`412 Precondition Failed`
* <a name="3.1.s4.b10"></a>不得对资源进行修改 

如果上述任何POST或DELETE请求情况下的报头前提条件失败，则LRS：

* <a name="3.1.s4.b11"></a>SHOULD *返回HTTP状态`412 Precondition Failed`。 
* <a name="3.1.s4.b12"></a>SHOULD*应该*不对资源进行修改。 

如果接收到PUT请求，但没有任何一个已经存在的资源的头，则LRS：

* <a name="3.1.s4.b13"></a>必须返回HTTP状态 `409 Conflict`.
* <a name="3.1.s4.b14"></a>必须返回一个解释学习记录提供者应该的响应
	* <a name="3.1.s4.b14.b1"></a>检查资源的当前状态
	* <a name="3.1.s4.b14.b2"></a>请使用当前ETag设置“If-Match”头以解决冲突
* <a name="3.1.s4.b15"></a>不得对资源进行修改

<a name="errorcodes" /> 

### <a name="3.2">3.2</a> Error Codes 错误代码

##### <a name="3.2.s1"></a>Description 描述

本规范定义了要求，其中一些要求强加于LRS以接受或拒绝请求，返回响应并在某些条件下执行其他行为。在需要使用LRS拒绝请求的情况下，将列出相应的错误代码作为需求的一部分。



这些要求中没有一个与LRS还被允许可配置为拒绝请求并且在超出本说明书的范围的情况下响应或行为不同的想法相矛盾。

这些条件之一是许可。例如，LRS可能会将权限分配给特定的凭据集，以便这些凭证只能发出与特定代理相关的语句。然后它可以拒绝使用与该代理无关的那些凭证的任何语句。除了第4.2节中建议的OAuth授权范围值的列表外，LRS可以分配的权限超出了本规范的范围。

权限还可以影响LRS向GET请求返回的响应。例如，一组凭据可能仅具有查看关于特定Actor的语句的权限，在这种情况下，LRS将过滤任何返回的语句以排除与该Actor无关的任何语句。有关详细信息，请参阅GET语句。

在本规范明确允许的情况下，使用的凭证还可能影响处理请求的LRS行为，例如LRS通常会覆盖Statement的“authority”属性，但有时可以接受提交的权限，如果它具有强信任关系与用于提交语句的凭据相关联。有关详细信息，请参阅权限。

由LRS设置的权限可能导致技术上符合的LRS失败一致性测试。这可能发生在由测试软件做出的请求基于权限被拒绝的情况下。因此，LRS需要是可配置的，或者用于测试的凭据需要授予足够的权限，以便权限限制不会影响一致性测试的结果。

另一个条件是发送的请求超出了LRS设置的大小限制。期望LRS始终接受任何大小的请求是不合理的。 LRS可以选择其认为合适的任何大小限制，但需要进行配置，以便在一致性测试期间不应用大小限制。当然，由于硬件等的限制，在一致性测试期间仍然存在一些大小限制，但是期望这些限制足够高，以便不影响测试的运行

LRS还可以在可疑的恶意意图的情况下拒绝请求或撤销凭证，例如在短时间内发出意外的大量请求。预期该限制将足够高，使得在一致性测试期间进行的请求的速率不会触发任何速率限制。

##### <a name="3.2.s2"></a>Details
下面的列表提供了一些有关可以从API中的各种方法返回的HTTP错误代码的一般性指导。
* <a name="3.2.s2.b1"></a>`400 Bad Request` - 指示由无效或缺少参数引起的错误状况。术语“无效参数”包括格式错误的JSON或无效的对象结构。

* <a name="3.2.s2.b2"></a>`401 Unauthorized` - 表示需要进行身份验证，或者在请求中发布了身份验证的情况下，拒绝了给定凭证。
* <a name="3.2.s2.b3"></a>`403 Forbidden` - 表示请求未授权给定凭证。注意这不同于拒绝给定的凭据。在这种情况下，已验证凭据，但不允许已验证的客户端执行给定的操作

* <a name="3.2.s2.b4"></a>`404 Not Found` - 表示找不到请求的资源。可以通过返回唯一标识的资源的任何方法返回，例如，针对特定文档的任何状态，代理配置文件或活动配置文件资源请求，或检索单个语句的方法。

* <a name="3.2.s2.b5"></a>`409 Conflict` - 指示在状态资源，代理配置文件资源或活动配置文件资源请求的情况下，或在语句资源PUT或POST调用中由于与资源的当前状态冲突的错误情况。有关更多详细信息，请参阅第3.1节并发。 [3.1 Concurrency](#concurrency) 

* <a name="3.2.s2.b6"></a>`412 Precondition Failed` - 指示在状态或代理配置文件或活动配置文件API请求的情况下，由于请求发布的前提条件失败而导致的错误条件。有关更多详细信息，请参见第6.3节。[6.3 Concurrency](#concurrency) 

* <a name="3.2.s2.b7"></a>`413 Request Entity Too Large` - 表示LRS已拒绝语句或文档，因为其大小（或请求中包含的附件大小）大于LRS允许的最大值。

* <a name="3.2.s2.b8"></a>`429 Too Many Requests` - 表示LRS已拒绝请求，因为它在给定时间内收到来自客户端的过多请求或一组凭证。

* <a name="3.2.s2.b9"></a>`500 Internal Server Error` - 表示一般错误条件，通常是服务器上的处理中的意外异常。

##### <a name="3.2.s3"></a>Requirements

* <a name="3.2.s3.b1"></a>LRS必须从上面的列表中返回最适合于错误条件的错误代码。

* <a name="3.2.s3.b2"></a>LRS应该在响应中返回一条消息，解释错误的原因。

* <a name="3.2.s3.b3"></a>LRS应该使用[RFC 7231](http://tools.ietf.org/html/rfc7231#section-5.3)中所述的内容协商来决定错误的格式。

* <a name="3.2.s3.b4"></a>LRS应该允许对错误的纯文本，HTML和JSON响应（使用内容协商）

* <a name="3.2.s3.b5"></a>学习记录提供者应该发送具有请求的“接受”报头以启用内容协商。

* <a name="3.2.s3.b6"></a>LRS应该拒绝具有400错误请求状态的任何请求，其中内容类型头部与请求中包括的内容不匹配，或者其中请求的结构与本说明书中针对特定内容类型概述的结构不匹配。例如，如果请求的内容格式为JSON，则内容类型应为 `application/json`。如果内容类型是application / x-www-form-urlencoded，则期望请求将包括如备用请求语法[Alternate Request Syntax](#alt-request-syntax)中概述的方法参数.

* <a name="3.2.s3.b7"></a> LRS必须拒绝`400 Bad Request`状态任何使用任何参数的请求，LRS在本规范的预期上下文中不能识别。 （注意：LRS可以识别并操作本规范中未提及的参数）。

* <a name="3.2.s3.b8"></a>LRS必须拒绝`400 Bad Request`状态任何使用任何参数匹配本规范中描述的参数的请求，除非情况。

* <a name="3.2.s3.b9"></a>如果该批次中的任何语句被拒绝，则LRS必须拒绝一批语句

* <a name="3.2.s3.b10"></a>LRS必须拒绝由LRS拒绝的任何请求的`403 Forbidden`，其中与请求相关联的凭证没有提出该请求的许可

* <a name="3.2.s3.b11"></a>如果有附件，声明或文档的大小大于LRS允许的最大值，则LRS必须拒绝`413 Request Entity Too Large`状态的任何请求被LRS拒绝。

* <a name="3.2.s3.b12"></a>LRS可以选择任何附件，声明和文件大小限制，并且可以在任何基础上（例如，每个权限）改变此限制

* <a name="3.2.s3.b13"></a>LRS必须拒绝`429 Too Many Requests`状态任何由LRS拒绝的请求，其中由于在给定时间量内特定客户端或一组凭证接收到太多请求而拒绝该请求。 
* <a name="3.2.s3.b14"></a>LRS可以选择任何速率限制，并且可以在任何基础上（例如，每个权限）改变此限制。

出于一致性测试的目的，存在以下要求，以确保由LRS实施的任何限制或权限不影响一致性测试软件的运行。

* <a name="3.2.s3.b15"></a>LRS应该可以配置为不根据权限拒绝来自特定凭证集合的任何请求。这组凭据应该用于一致性测试，但可以在活动系统上删除/禁用

* <a name="3.2.s3.b16"></a>LRS必须可配置为接受任何合理大小的附件，语句或文档（见上文）。

* <a name="3.2.s3.b17"></a>LRS必须可配置为以任何合理的速率接受请求。






<a name="Appendix3B"/>

### <a name="B">Appendix B</a>: Table of All Resources

### <a name="B.s1"></a>Required Resources
<table>
	<tr>
		<th>Base Resource Endpoint of the LRS Precedes Each Endpoint</th>
		<th>Function</th>
	</tr>
	<tr id="B.s1.table1.row1">
		<td>statements</td>
		<td>Statement Storage/Retrieval</td>
	</tr>
	<tr id="B.s1.table1.row2">
		<td>agents</td>
		<td>Agent Object Storage/Retrieval</td>
	</tr>
	<tr id="B.s1.table1.row3">
		<td>agents/profile</td>
		<td>Agent Profile Resource</td>
	</tr>
	<tr id="B.s1.table1.row4">
		<td>activities</td>
		<td>Activity Object Storage/Retrieval</td>
	</tr>
	<tr id="B.s1.table1.row5">
		<td>activities/profile</td>
		<td>Activity Profile Resource</td>
	</tr>
	<tr id="B.s1.table1.row6">
		<td>activities/state</td>
		<td>State Resource</td>
	</tr>
	<tr id="B.s1.table1.row7">
		<td>about</td>
		<td>LRS Information</td>
	</tr>
</table>

### <a name="B.s2"></a>OAuth Resources
<table>
	<tr>
		<th>Base Resource Endpoint of the LRS Precedes Each Endpoint</th>
		<th>Function</th>
	</tr>
	<tr id="B.s2.table1.row1">
		<td>OAuth/initiate</td>
		<td>Temporary Credential Request</td>
	</tr>
	<tr id="B.s2.table1.row2">
		<td>OAuth/authorize</td>
		<td>Resource Owner Authorization</td>
	</tr>
	<tr id="B.s2.table1.row3">
		<td>OAuth/token</td>
		<td>Token Request</td>
	</tr>
</table>

<a name="Appendix3C"/>

### <a name="C">Appendix C</a>: Cross Domain Request Example

[Alternate Request Syntax](#alt-request-syntax) outlines alternative syntax for use when the normal syntax cannot be used due 
to browser or querystring length restrictions. This appendix provides an example of a PUT request to the Statements Resource 
following this format. 

Request using normal syntax:

```
URL: http://example.com/xAPI/statements
Method: PUT

Query String Parameters:
    statementId=c70c2b85-c294-464f-baca-cebd4fb9b348

Request Headers:
    Accept:*/*
    Accept-Encoding:gzip, deflate, sdch
    Accept-Language:en-US,en;q=0.8
    Authorization: Basic VGVzdFVzZXI6cGFzc3dvcmQ=
    Content-Type: application/json
    X-Experience-API-Version: 1.0.3
    Content-Length: 351

Content:
{"id":"c70c2b85-c294-464f-baca-cebd4fb9b348","timestamp":"2014-12-29T12:09:37.468Z","actor":{"objectType":"Agent","mbox":"mailto:example@example.com","name":"Test User"},"verb":{"id":"http://adlnet.gov/expapi/verbs/experienced","display":{"en-US":"experienced"}},"object":{"id":"http://example.com/xAPI/activities/myactivity","objectType":"Activity"}}

```

Request using alternative syntax:

```
URL: http://example.com/xAPI/statements?method=PUT&statementId=c70c2b85-c294-464f-baca-cebd4fb9b348
Method: POST

Request Headers:
    Accept:*/*
    Accept-Encoding:gzip, deflate, sdch
    Accept-Language:en-US,en;q=0.8
    Content-Type: application/x-www-form-urlencoded
    Content-Length: 745

Content (with added line breaks and not URL encoded for readability):
    statementId=c70c2b85-c294-464f-baca-cebd4fb9b348
    &Authorization=Basic VGVzdFVzZXI6cGFzc3dvcmQ=
    &X-Experience-API-Version=1.0.3
    &Content-Type=application/json
    &Content-Length=351
    &content={"id":"c70c2b85-c294-464f-baca-cebd4fb9b348","timestamp":"2014-12-29T12:09:37.468Z","actor":{"objectType":"Agent","mbox":"mailto:example@example.com","name":"Test User"},"verb":{"id":"http://adlnet.gov/expapi/verbs/experienced","display":{"en-US":"experienced"}},"object":{"id":"http://example.com/xAPI/activities/myactivity","objectType":"Activity"}}
```
