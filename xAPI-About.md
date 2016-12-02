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
	*	1.0.	[Introduction 介绍](./xAPI-About.md#introduction-partone) 
	*	2.0.	[How To Use This Document 如何使用本文档](./xAPI-About.md#readingguidelines)  
		*	2.1.	[MUST / SHOULD / MAY](./xAPI-About.md#def-must-should-may)  
	 	*	2.2.	[Guidelines for Interpreting Descriptive Text and Tables 解释描述性文本和表的指南](./xAPI-About.md#interpret-text-table)  
	*	3.0.	[Serialization and JavaScript Object Notation 数据序列化（格式化）和JavaScript 对象标记（JSON）](./xAPI-About.md#json)
	*	4.0.	[Definitions 定义](./xAPI-About.md#definitions) 
	*	5.0.	[xAPI Components 组件](./xAPI-About.md#xapi-components) 
	*	6.0.	[Extending xAPI 扩展](./xAPI-About.md#extending-xapi) 
	*	7.0.	[Profiles and Communities of Practice 预配置和xAPI社区](./xAPI-About.md#COPs)  
	*	[Appendices 附录](./xAPI-About.md#append1)  
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

<a name="partone" />
#Part One: About the Experience API

<a name="introduction-partone"></a>
## 1.0 介绍


xAPI 是一个技术规范，旨在促进学习体活动的文档化和交流。 它规定了一种描述学习活动的数据结构，并定义如何以电子方式交换这些描述数据。

<br>

xAPI 是由  Advanced Distributed Learning (ADL)起草的。ADL成立于1997年，旨在实现美国教育的培训，管理及交付的标准化和现代化。在评估某人对某个职位的适应性和其执行任务的能力过程中，对于该人的评价往往是需要广泛的考虑正式的教育背景（学位）和非正式的学习活动（Mook），而这些信息通常是分散在各个平台来源中。从那个时候起，越来越多人意识到跟踪个人学习活动及其经历的重要性。

<br>

正是这种需求，催生了xAPI的社区和规范，xAPI的应用情况
  * 客观的有需要对分散在分离的平台上的学习活动和历史信息的分析。
  *为了实习这一目标，最佳的方式是开发一个广为接受的信息收集，储存和交换的框架。

xAPI的目标:

* 使得在各种不同的环境，平台和技术中，更加容易的来比较和获得学习活动，学习记录以及学习结果。
* 最大限度地提高创建，收集，存储和处理学习体验信息的服务的互操作性。
* 为希望构建符合并实现本规范的应用程序的用户提供指南。
* 提供可以测试符合本规范的标准。

本文档给出的规范都是设计来达成上面的目标的。
<a name="readingguidelines"></a>

## 2.0 如何使用本文档

这是一个明确描述如何实施xAPI的文档，。 它是专门针对实施此技术的个人和组织编写的技术文档，其目的是开发可互操作的工具，系统和服务，这些工具，系统和服务彼此独立并且可以互相操作。 

<br>

在可能的情况下，本文档中使用的语言和格式旨在考虑非技术读者，对于各种工具，系统和服务的相应部分的描述， xAPI的文档的给定方面将高级概述的部分标记了出来，因此本文件中标记为**要求**，**细节**或**示例**的项目更具技术性。

<br>

本规范分为三部分。 第一部分是这个介绍。 它提供了一些背景，高级摘要和如何阅读规范的其余部分。 

<br>


本规范的第二部分定义了本规范中使用的各种数据对象的数据模型。xAPI数据模型中最重要的对象是“Statement”对象。此规范定义了Statement对象（包括 “Actor”，“Verb”，“Object”，“Result”和“Context”）的属性以及这些属性的值及其表示方式的语法规则。这部分有助于确保实现规范的服务遵循一致的数据结构。

<br>


本规范的第三部分阐述了在遵守规范的服务之间传达学习经验的信息时必须使用的传输方法。 这包括请求的格式和预期的响应。 注意，xAPI中的通信不仅限“学习记录存储库”（LRS）从“内容”接收数据。 LRS还可以与“学习记录提供者”和“学习记录消费者”的服务或与其他LRS进行通信。 xAPI遵循REST软件架构风格的指导原则，因此数据通过HTTP请求和响应传输。 第三部分还定义如何了让LRS和可信“客户端”之间进行可信任的，安全的交换信息的方法。

<a name="def-must-should-may"></a>
### 2.1 MUST / SHOULD / MAY 
关于标识的xAPI规范的遵守，有三个级别，MUST，SHOULD和MAY。 不满足MUST（或MUST NOT）的要求的服务或系统，是不符合规范要求的。不满足SHOULD要求的不违反规范性，但违反规范的建议。 MAY表示一个选项，由开发人员决定，没有一致性的后果。文档尽可能避免在限定语句之外的地方使用这些术语，文档中在限定语句之外的地方使用这些术语的，不表达指定要求的意义。 可以在[RFC 2119](https://www.ietf.org/rfc/rfc2119.txt)中找到MUST，SHOULD，MAY，MUST NOT和SHOULD NOT的完整定义。 

<br>

在SHOULD之后使用星号*的标记表示非常强烈的建议。 计划在未来版本中这些建议将成为MUST要求。 不遵循这些建议可能会有互操作性风险和/或导致其他各种问题，具体取决于建议的具体情况。 这些建议在本版本中不是MUST要求，是因为将来有可能重定义或者更改。 xAPI工作组强烈建议使用者实施这些要求，就像它们是必须要求的，同时也支持可能不这样做的其他使用者。

<br>

<a name="interpret-text-table"></a>
### 2.2 解释描述性文本和表的指南
作为一个首要的法则，如果指南看起来是技术性的或是必须性的，则将其解释解析成列表一样的一系列要求。这可能有一点复杂，尤其是对于越长，越详细的解释和列表，越有可能不直观且冗长。

<br>

在本规范书中使用列表来定义属性，参数等的限制和描述。列表定义了哪些属性是必需的，推荐的和可选的。 通常，对于属性，参数等，“可选”的概念涉及创建对象的服务，而接收和解析对象的服务需要能够解析该对象的所有属性。 通常，属性是可选的，因为数据在一些上下文中可能不相关; 如果数据在特定上下文中是相关的，则期望使用该属性。

<br>

如果可选属性或参数包含的对象拥有推荐的变量，并且这些变量被确实使用了，那么这些可选属性是被推荐来使用的。

<br>

在整个说明书和附录中提供了示例以说明如何实现。 这些示例的内容是虚构的，以便说明本规范书的要求，并且可能不总是示出跟踪示例中使用的特定学习经验的实践方法。 示例可用于说明需求的解释，但不意图优先于需求。整个说明书和附录中提供了示例以说明实现。

<br>

关于实施的特定方面的要求，凡本规范中不包括的，这个部分就被认为是超出范围的标准。由实施者来确定是较为妥当的。本规范试图避免模糊性，即使在某一领域没有说明，通常也会给出一个理由。

<br>

<a name="json"></a>
## 3.0 数据序列化（格式化）和JavaScript 对象标记（JSON）

序列化是将数据对象和结构翻译成方便存储或传输的数据的过程，并且使得该原始数据对象可以从所翻译得到到的序列中重新解读出来。在一些情况下，可能有多种方式来序列化某段数据，例如一个为ture布尔属性，取决于方法，它的值可以被表达为`1`或者`true`。 

<br>

xAPI遵循JSON数据化格式（所以布尔值表示为`true`或者`false`）.但是xAPI是支持其他数据序列化方法的，例如XML，但在这里超出了,本说明的讨论范围，所以不予讨论。

<br>

尽管JSON本身对于数据格式的限制是可能变化的，特别是关系到时间的数据。这里作为xAPI的一大优点就是系统依然能分辨两个语句（Statement)是否相同。关于更多的对于语句这方面影响，查看不变性和异常。[Immutability and exceptions](./xAPI-Data.md#statement-immutability-and-exceptions)

<br>

JSON 允许对象的属性包含一个空的对象，而这在xAPI中是不推荐这样做的；如果一个语句中的某个属性不包含对象的话，那么这个属性就根本没有用，所有的属性都需要包含一个具体值。

<br>


<a name="definitions"></a>
## 4.0 Definitions 定义

* [Activity](#def-activity) 活动
* [Activity Provider (AP)](#def-activity-provider) 活动提供方
* [Actor](#def-actor) 执行者
* [Application Programming Interface (API)](#def-api) 应用程序接口
* [Authentication](#def-authentication) 认证
* [Authorization](#def-authorization) 授权
* [Community of Practice](#def-community-of-practice) xAPI实践社区
* [Document Profile Resource](#def-document-profile) 配置文件源
* [Endpoint](#def-endpoint) 端点
* [Experience API (xAPI)](#def-experience-api)
* [Immutable](#def-immutable) 不变性
* [Internationalized Resource Identifier (IRI)](#def-iri) 国际化资源标识符
* [Internationalized Resource Locator (IRL)](#def-irl) 国际化资源定位符
* [Inverse Functional Identifier](#def-inverse-functional-identifier) 反向功能标识符
* [Learning Experience](#def-learning-experience) 学习经历活动
* [Learning Management System (LMS)](#def-learning-management-system) 学习管理系统
* [Learning Record](#def-learning-record) 学习记录
* [Learning Record Consumer (LRC)](#def-learning-record-consumer) 学习记录客户
* [Learning Record Provider (LRP)](#def-learning-record-provider) 学习记录供应商
* [Learning Record Store (LRS)](#def-learning-record-store) 学习记录存储
* [Metadata Consumer](#def-metadata-consumer) 元数据消费者
* [Metadata Provider](#def-metadata-provider) 元数据提供者
* [Persona](#def-persona) 身份
* [Profile](#def-profile) 预配置
* [Registration](#def-registration) 注册
* [Representational State Transfer (REST)](#def-rest) 具象状态传输
* [Service](#def-service) 服务
* [Statement](#def-statement) 语句
* [Tin Can API (TCAPI)](#def-tcapi)
* [Verb](#def-verb) 行动
* [Vocabulary](#def-vocabulary) 术语词汇集 

<a name="def-activity" ></a>

__Activity 活动__: 一类组成“I Did This”中This的对象，表示一些学习活动，可以是一项与动词组合起来具有追中意义的指令，经历，或者行为。Activity的解释很广，意味着也有可能是有实际概念的物体，如椅子（真实的或者虚拟的），在“安娜尝试了某个蛋糕配方”这个语句中，配方作为Activity构成了xAPI的语句。Activity的其他例子例如一个电子课程，一次远足，或者一次例会等。

<br>

<a name="def-activity-provider" ></a>

__Activity Provider (AP)活动提供方__: 现在被称为学习记录提供方（Learning Record Provider）。这是为了区分某活动本身的软件提供者并不总是该条信息的提供者。

<br>

<a name="def-actor" ></a>

__Actor 执行者__:一个个人或者一个群体，代表着被记录者。 在“I did this”中表示“I”；

<br>

<a name="def-api" ></a>

__Application Programming Interface (API) 应用程序接口__: 一组创建允许访问到软件应用程序或工具的规则和标准。

<br>

<a name="def-authentication" ></a>

__Authentication 认证__: 表示证明双方“信任”

<br>

<a name="def-authorization" ></a>

__Authorization 授权__: 根据角色来给予一些操作权利。

<br>

<a name="def-client" ></a>

__Client 用户__: 指代任何有可能有需求的实体，例如一个学习记录提供方(earning Record Provider)，学习记录购买方(Learning Record Consumer)，一个学习记录库(Learning Record Store (LRS)），或者一个学习管理系统 (Learning Management System (LMS)).

<br>

<a name="def-community-of-practice" ></a>

__Community of Practice (CoP) xAPI实践社区__: 一个关于某个特定用例的xAPI社区，旨在为这种特定用例建立vocabularies, profiles, and recipes.

<br>

<a name="def-document-profile" ></a>

__Document Profile Resource 配置文件源，__: 一个保存了关于学习者或者活动信息的的构造，通常是对某个教学系统有用的一个文档，不要与[Profile配置](#def-profile)混淆。 

<br>

<a name="def-endpoint" ></a>

__Endpoint 端点__: 面向服务的架构中的入口点。 xAPI通过定义与其进行通信的IRI作为端点，将此方法与资源进行镜像。

<br>

<a name="def-experience-api" ></a>

__Experience API (xAPI)__: 本文档中阐述的规则集合，确定如何定义，格式化和交换学习体验，以便独立软件程序可以交换和使用此信息。

<br>

<a name ="def-immutable" ></a>

__Immutable 不变性__:  一个形容词，用来描述不能改变的特性。 除了一些例外，xAPI中的语句是不可变的。 这确保了当LRS之间共享语句时，语句的多个副本保持不变。

<br>

<a name="def-iri" ></a>

__Internationalized Resource Identifier 国际化资源标识符  (IRI)__: 可以是IRL的唯一标识符。 用于标识对象，如动词(Verb)，活动(Activity)或活动类型。 与URI不同，IRI可以包含ASCII字符集之外的一些字符，以支持国际语言。 

<br>

IRI总是包括一个方案。 这不是此标准的要求，而是IRI的定义的一部分，根据[RFC 3987](http://www.ietf.org/rfc/rfc3987.txt).有时称为“相对IRI”的不是IRI。

<br>


<a name="def-irl" ></a>

__Internationalized Resource Locator (IRL) 国际化资源定位符__:  在本文档的上下文中，IRL是一个IRI，当翻译为URI（根据IRI到URI规则）时，它是一个URL。 

<br>

<a name="def-inverse-functional-identifier" ></a>

__Inverse Functional Identifier 反向功能标识符__: 对特定人员或群体的唯一标识符。

<br>

<a name="def-learning-experience" ></a>

__Learning Experience 学习经历(活动)__: 与学习相关的事件。 它是高度多样化的。例如，阅读一本书，参加在线课程，参加实地考察，参加自我指导的研究，或接收完成课程的证书。

<br>

<a name="def-learning-management-system" ></a>

__Learning Management System 学习管理系统 (LMS)__: “针对一个或多个学习者，用于管理一个或多个课程的LMS，通常是一个基于网络的系统，允许学习者认证自己，注册课程，完成课程和进行评估” （学习系统架构实验室定义）。 对于本文档的LMS，把在系统内如何将用户识别为“受信任”并且能够访问其学习体验作为示例。

<br>

<a name="def-learning-record" ></a>

__Learning Record 学习记录__: 由xAPI规定的形式来表示学习活动的一个账户的数据。一个学习记录可以有多种形式，包括语句，文件，及其他部分。这些都可以称为学习记录。

<br>

<a name="def-learning-record-consumer" ></a>

__Learning Record Consumer 学习记录客户 (LRC)__: 作为xAPI的使用者，客户端，以应用学习记录储存库LRS中的数据为主要目的，包括解释，分析，翻译和传播等。

<br>

<a name="def-learning-record-provider" ></a>

__Learning Record Provider 学习记录供应商 (LRP)__:  同样作为xAPI的一个客户端，以创建学习记录并发送到学习记录储存库LRS为主要目的，通常为所被记录学习者学习的一些服务商。

<br>

<a name="def-learning-record-store" ></a>

__Learning Record Store 学习记录存储 (LRS)__: 一个服务器（即能够接收和处理Web请求的系统）负责接收，存储和提供访问学习记录。

<br>

<a name="def-metadata-consumer" ></a>

__Metadata Consumer 元数据消费者__: 一个人，组织，或软件，旨在，查看或是获取由本规范中所定义的IRI所解析出的元数据或与其相关的东西。一个LRS可能是也可能不是一个元数据的消费者。

<br>

<a name="def-metadata-provider" ></a>

__Metadata Provider 元数据提供者__: 一个人，组织，或软件程序，以一定价格将由本规范中所定义的IRI所解析出的元数据作为服务的提供者。

<br>

<a name="def-persona" ></a>

__Persona 身份__: 一组唯一定义了一个执行者的一个或多个表示。从概念上讲，这就像有一个“生活电子邮件”和“工作电子邮件”。两者虽然是同一个人，但有不同的数据，联系作用等。

<br>

<a name="def-profile" ></a>

__Profile 预配置__:一组简单描述如何实施xAPI的文档。预配置一般提供一些术语来解释特定词汇，一些是专门为预配置所创建的，有些是从其它词汇中引用过来的。有时，一个预配置可能针对不同情况提供多个解释，有时有人会解释来自多个来源的同一个词汇，而无需创建一个新的预配置。不要与文档配置资源[Document Profile Resource](#def-document-profile)相混淆。 

<br>

<a name="def-registration" ></a>

__Registration 注册__: 一个当事人去经历一个特定的活动的实例。

<br>

<a name="def-rest" ></a>

__Representational State Transfer 具象状态传输 (REST)__: 用于设计网络Web服务的架构。它依赖于HTTP方法和使用当前最佳的网络规范。

<br>

<a name="def-service" ></a>

__Service 服务__: 一个软件或者系统负责提供离散式学习的某个方面。一个典型的例子就是一个LMS集成了多个服务，从而实现管理完整的学习活动。

<br>

<a name="def-statement" ></a>

__Statement 语句__: 用于表达任何形式的学习活动或事件的语法结构。成组的有着相应时间的语句则用来描述某个学习活动的详细信息。 

<br>

<a name="def-tcapi"></a>

__Tin Can API (TCAPI)__: xAPI的另外一个名字。

<br>

<a name="def-verb" ></a>

__Verb 行动__: 由当事人（学习者）所执行的的某个动作，在“I did this”语句结构中作为did。

<br>

<a name="def-vocabulary" ></a>

__Vocabulary 术语词汇__:一个包含了特定领域术语的集合。旨在规范每个人都使用同样的词汇，从而方便理解和交流。请参阅xAPI词汇规范 [xAPI Vocabulary Companion Specification](https://github.com/adlnet/companion-specification-for-xapi-vocabularies/blob/master/SUMMARY.md)。

<br>

<a name="xapi-components" ></a>

## 5.0 xAPI Components 组件

这个部分图像化的解释和展示了xAPI的各个部分是如何应用到一起的。

##### 追踪学习经历

###### Figure 1: xAPI数据流
![Data Flow in xAPI](./xAPIDataFlow.jpg)

图1给出了跟踪学习记录的过程，一个学习者在学习过程中会有学习活动，这可能是发生在一个慕课网站（在线网络教育）中，也有可能是工作中，更甚于在娱乐活动中。然后这个活动被受信任的学习记录提供商追踪，从而代表着学习者的经历。这可能是某个学习者开始去执行了某个内容，与内容的完成度等等。

<br>

学习记录提供商创建学习记录然后发送到一个或者多个LRS中，然后这个LRS将这些数据保存下来，然后给予受信任的第三方访问权限，从而受信任的第三方(学习记录消费者)根据这些数据来管理，推送，执行合适的内容或者其他操作。

<br>

##### 活动数据和元数据

###### Figure 2: xAPI活动数据和元数据
![xAPI Activity Data and Metadata](./xAPIMetadata.jpg)

在xAPI中，理解如何来定义和描述一个活动（由一个唯一IRI标识）是一个非常关键的概念 图2展示了这个过程。一个活动（作为语句的一部分）有着相应的元数据，这些数据有可能是语句本身定义，这是由语句活动定义规范定义的。对于每一个活动的id，都是一个IRI，而在这个IRI的对应解析地址下也可能有元数据。任何IRI所解析的元数据都在元数据提供者的控制之下，而元数据提供者也呀负责确保IRI的长期存在和解析的正确性。

<br>

任何位于由IRI所解析地址的元数据都是关于元数据的权威性资源。可以被用于作为LRS规范的对于相应活动的元数据的定义，和解析参考。一个元数据消费者可以通过IRI访问权威性版本的元数据，或者查询活动元数据的典范版本。

<br>

##### 代理和身份管理

###### Figure 3: xAPI代理和身份管理
![xAPI Activity Data and Metadata](./xAPIPersonas.jpg)

xAPI 提供了允许选择性的访问某人的个人信息的框架。这是通过被称为“身份”的管理系统所实现的。在xAPI中，每一个身份代表着“I”在“I did this”语句中，作为逻辑上的主语。每一个代理或团体在xAPI中对应一种身份，某个学习者发送了一条学习记录到一个LRS可以是通过多重身份的。

<br>

在图3中，一个学习者访问多种服务，其中的一些是在工作中，其余的是在家里，一些是为了社交，另一些是为了教育或者私人原因。所以说这些服务的功能是基于不同身份的，每一个服务都会给LRS发送数据，之后，就会有以三种不同身份的三条记录存于LRS中，而它们属于同一个人

<br>

LRS能将对于多重身份的所有信息都整合到一个“人”对象中，而这个对象能通从LRS中通过[Agents Resource 代理资源](./xAPI-Communication.md#agentsres)而被解析出来，LRS怎么能知道这些多重身份属于某个人在这里不做讨论。 

<a name="extending-xapi" ></a>

## 6.0 Extending xAPI xAPI扩展

xAPI 能在多方面进行扩展，最值得注意的是语句的扩展，对于语句有着巨大的灵活性。对于特定的用例和应用配置，推荐使用xAPI社区认可的扩展。实现详细信息请参考[4.1 Extensions](./xAPI-Data.md#miscext).

<br>

另外一个可扩展的例子是About信息，LRS的交互优势可能超过本申明所及。扩展LRS的说明信息可以对社区带来贡献。

<br>

最后，对于本xAPI资源的实施并不仅限于本文档所描述。超出本文档所列出的措施之外的可实施措施也是可行的。

<a name="COPs" ></a>

## 7.0 Profiles, Vocabularies, and Communities of Practice

xAPI 严格定了的语句的结构，但是以该结构为基础的内容却非常的灵活，例如，本规范要求所有的语句必须包含一个“verb”属性，但是并没有限制这个属性的值，任何“动作”都可以视同。这种灵活性给了xAPI足够的应用空间来适应未来的用例。

<br>

xAPI社区[Communities of Practice (CoPs)](#def-community-of-practice)在他们的配置文件里定义Verb、Activity 类型，上下文关系，扩展等的意图是为了在可以应用的情况中提供一个唯一的标识。xAPI社区将这些标识和他们的元数据定义到了词汇集[Vocabulary](#def-vocabulary)中。一个配置文件是一系列为了满足特定用例而需要被实现的规则和词汇。它一个非常有利于社区的重要的实施方式，寻求更多有关于已发布词汇集，请阅览伴随词汇规范[Vocabulary Companion Specification](https://adl.gitbooks.io/companion-specification-for-xapi-vocabularies/content)文档和词汇入门[Vocabulary Primer](https://adl.gitbooks.io/experience-xapi-vocabulary-primer/content/)文档。

<br>


推荐对于一个配置情形使用一个唯一的“分类”，并且提供一个具体的语句实例作为参考。一个典范配置清醒是cmi5，一个设计给传统个人学习者的线上学习用例。你可以在附录B
Cmi5 实例中查看。 [Appendix B: cmi5 Example](#Appendix1B).

<br>

多利用xAPI社区资源是非常推荐的，这样可以避免进行重复工作，就是说用不同的方式来解决同一个问题，这会带来在同类领域的碎片化，并且可能伤害互操作性。这里有一个关于医学领域的实例 [MedBiquitous Learning Experience Working Group](http://groups.medbiq.org/medbiq/display/XIG/Learning+Experience+Group+Home).


<a name="append1"></a>
## 附录



<a name="Appendix1B"></a>
### Appendix B: cmi5 Example 

The following example illustrates a statement following the cmi5 Community of Practice. It demonstrates use of extensions 
and "category" contextActivities.

下面的例子展示了一个语句是如何按cmi5社区所规范的配置来构建的，还演示了扩展的运用和“分类”内容。

```
{  
  "id":"2a41c918-b88b-4220-20a5-a4c32391a240",
  "actor":{  
    "objectType":"Agent",
    "name":"Gert Frobe",
    "account":{  
      "homePage":"http://example.adlnet.gov",
      "name":"1625378"
    }
  },
  "verb":{  
    "id":"http://adlnet.gov/expapi/verbs/failed",
    "display":{  
      "en-US":"failed"
    }
  },
  "object":{  
    "id":"https://example.adlnet.gov/AUidentifier",
    "objectType":"Activity"
  },
  "result":{  
    "score":{  
      "scaled":0.65,
      "raw":65,
      "min":0,
      "max":100
    },
    "success":false,
    "duration":"PT30M",
    "extensions":{  
      "https://w3id.org/xapi/cmi5/result/extensions/progress":100
    }
  },
  "context":{  
    "registration":"ec231277-b27b-4c15-8291-d29225b2b8f7",
    "contextActivities":{  
      "category":[  
        {  
       	  "id":"https://w3id.org/xapi/cmi5/context/categories/moveon"
        },
        {  
          "id":"https://w3id.org/xapi/cmi5/context/categories/cmi5"
        }
      ]
    },
    "extensions":{  
      "https://w3id.org/xapi/cmi5/context/extensions/sessionid":"458240298378231"
    }
  },
  "timestamp":"2012-06-01T19:09:13.245+00:00"
}
```

