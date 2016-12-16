
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
*	Part Two:	[Experience API Data  XAPI 数据](./xAPI-Data.md#parttwo) 
	*	1.0.	[Documents 文档](./xAPI-Data.md#documents) 
	*	2.0.	[Statements  语句](./xAPI-Data.md#statements) 
		*	2.1.	[Purpose 目的](./xAPI-Data.md#statement-purpose)  
	 	*	2.2.	[Formatting Requirements 格式要求](./xAPI-Data.md#dataconstraints) 
	 	*	2.3.	[Statement Lifecycle 语句生态](./xAPI-Data.md#lifecycle) 
		 	*	2.3.1.	[Statement Immutability 语句不变性](./xAPI-Data.md#statement-immutability-and-exceptions) 
		 	*	2.3.2.	[Voiding 无效化](./xAPI-Data.md#voided) 
   		*	2.4.	[Statement Properties 语句的属性](./xAPI-Data.md#statement-properties)  
	        *	2.4.1.	[ID](./xAPI-Data.md#stmtid)  
	        *	2.4.2.	[Actor 执行者](./xAPI-Data.md#actor)  
	        *	2.4.3.	[Verb 动词](./xAPI-Data.md#verb)   
	        *	2.4.4.	[Object 对象（宾语）](./xAPI-Data.md#object)  
	        *	2.4.5.	[Result 结果](./xAPI-Data.md#result)  
	        *	2.4.6.	[Context 内容](./xAPI-Data.md#context)  
	        *	2.4.7.	[Timestamp 时间戳](./xAPI-Data.md#timestamp)   
	        *	2.4.8.	[Stored 储存（时间点）](./xAPI-Data.md#stored) 
	        *	2.4.9.	[Authority 授权](./xAPI-Data.md#authority)  
	        *	2.4.10.	[Version 版本](./xAPI-Data.md#version)  
	        *	2.4.11.	[Attachments 附件](./xAPI-Data.md#attachments)  
    	*	2.5.	[Retrieval of Statements 语句的检索](./xAPI-Data.md#retrieval)   
    	*	2.6.	[Signed Statements 语句的签名](./xAPI-Data.md#signature)  
	*	3.0.	[Metadata 元数据](./xAPI-Data.md#metadata) 
		*	3.1.	[IRI Requirements 对IRI的要求](./xAPI-Data.md#iri-requirements)  
		*	3.2.	[Hosted Metadata 站点元数据](./xAPI-Data.md#miscmeta)  
    *	4.0.	[Special Data Types and Rules 特殊的数据和规则](./xAPI-Data.md#special-data)  
		*	4.1.	[Extensions 扩展](./xAPI-Data.md#miscext) 
		*	4.2.	[Language Maps 语言映射](./xAPI-Data.md#lang-maps) 
		*	4.3.	[IRIs 国际化资源定位符 IRIs](./xAPI-Data.md#iris) 
		*	4.4.	[UUIDs](./xAPI-Data.md#uuids) 
		*	4.5.	[ISO 8601 Timestamps ISO 8601时间戳](./xAPI-Data.md#timestamps) 
		*	4.6.	[ISO 8601 Durations  ISO 8601持续时间](./xAPI-Data.md#durations)
	*	[Appendices 附录2](./xAPI-Data.md#append2)  
		*	[Appendix A: Example Statements 语句示例](./xAPI-Data.md#Appendix2A)  
		*	[Appendix B: Example statement objects of different types 语句对象（宾语）的不同种类示例](./xAPI-Data.md#Appendix2B)  
		*	[Appendix C: Example definitions for Activities of type "cmi.interaction" cmi交互示例](./xAPI-Data.md#Appendix2C)  	
		*	[Appendix D: Example Signed Statement 语句签名示例](./xAPI-Data.md#Appendix2D)  
*	Part Three:	[Data Processing, Validation, and Security 第三部分 数据的传输，验证，和安全](./xAPI-Communication.md#partthree)  
	*	1.0.	[Requests](./xAPI-Communication.md#requests)
		*	1.1.	[HEAD Request Implementation HEAD 请求申明](./xAPI-Communication.md#httphead)  
	 	*	1.2.	[Headers 头](./xAPI-Communication.md#headers) 
	 	*	1.3.	[Alternate Request Syntax 备选句法](./xAPI-Communication.md#alt-request-syntax) 
	 	*	1.4.	[Encoding 编码](./xAPI-Communication.md#encoding) 
	 	*	1.5.	[Content Types 内容类型](./xAPI-Communication.md#content-types) 
	        *	1.5.1.	[Application/JSON](./xAPI-Communication.md#applicationjson) 
	        *	1.5.1.	[Multipart/Mixed](./xAPI-Communication.md#multipartmixed)
	*	2.0.	[Resources](./xAPI-Communication.md#datatransfer)   
	 	*	2.1.	[Statement Resource 语句资源](./xAPI-Communication.md#stmtres) 
	 	*	2.2.	[Documents Resources 文档资源](./xAPI-Communication.md#doctransfer) 
	 	*	2.3.	[State Resource 状态资源](./xAPI-Communication.md#stateres) 
	 	*	2.4.	[Agents Resource 代理资源](./xAPI-Communication.md#agentsres) 
	 	*	2.5.	[Activities Resource 活动资源](./xAPI-Communication.md#activitiesres) 
	 	*	2.6.	[Agent Profile Resource 代理配置资源](./xAPI-Communication.md#agentprofres) 
	 	*	2.7.	[Activity Profile Resource 活动配置资源](./xAPI-Communication.md#actprofres) 
	 	*	2.8.	[About Resource 关于资源](./xAPI-Communication.md#aboutresource)
	*	3.0.	[Data Validation 数据验证](./xAPI-Communication.md#validation)
	*	3.1.	[Concurrency 并发](./xAPI-Communication.md#concurrency)
	*	3.2.	[Error Codes 错误代码](./xAPI-Communication.md#errorcodes)
    	
	*	[Appendices](./xAPI-Communication.md#append3)  
		*	[Appendix A: Converting Statements to 1.0.0](./xAPI-Communication.md#Appendix3A)  
		*	[Appendix B: Table of All Resources](./xAPI-Communication.md#Appendix3B)  
		*	[Appendix C: Cross Domain Request Example](./xAPI-Communication.md#Appendix3C)  


<a name="parttwo" />
#Part Two: Experience API Data

<a name="documents" />
## <a name="1.0">1.0</a> Documents 文本

xAPI为LRP学习记录提供者提供了能够以文档的形式储存任意数据的功能，这些数据在很大程度上是非结构化的，具有灵活性。关于这方面的细节可以在第三部分中找到。 [Part 3](./xAPI-Communication.md#doctransfer) 

<a name="statements" /> 

## <a name="2.0">2.0</a> Statements  语句

<a name="statement-purpose"/> 
### <a name="2.1">2.1</a> Purpose 意图

语句是被xapi追踪的任何学习活动的证明， 语句不仅能被容易的用自然语言来描述，也能按照JSON 来被计算机识别，这在设计过程中是十分有用的。语句是被用来做分析和整合的，而这在整个xapi中都是很关键的。

<a name="dataconstraints"/>
### <a name="2.2">2.2</a> Formatting Requirements 语法要求

###### <a name="2.2.s1"></a>Details

语句中使用的所有属性限于某些数据类型。 为了清楚起见，这里记录了关键要求，强调xAPI组件以规范的方式采取行动。

###### <a name="2.2.s2"></a>Requirements 要求

* <a name="2.2.s2.b1"></a>语句和其他对象 不可SHOULD NOT 包括一个空值或者空对象
* <a name="2.2.s2.b2"></a>一条语句 对于一个属性的使用 必须MUST 不能超过一次
* <a name="2.2.s2.b3"></a>一条语句 必须MUST 使用主 谓 宾
* <a name="2.2.s2.b4"></a>一条语句 可能 MAY 以任何顺序使用他的多个属性
* <a name="2.2.s2.b5"></a>除了被列出来的这些的属性[listed as exceptions](#statement-immutability-and-exceptions) LRS 学习记录存储库  MUST NOT不能返回不同的属性序列 


###### <a name="2.2.s3"></a>Learning Record Provider Requirements 对学习记录提供者的要求

为了强调和明确，以及提供一个开发指导，下面的要求特别限制了已经在其他地方包含了的重要要求。一些类型的验证，例如IRI的验证和对属性只能使用一次的验证，是非常不一样的。所以许多确保数据可移植性的负担在学习记录提供者（Learning Record Provider）上。

* <a name="2.2.s3.b1"></a>IRI需要的变量必须与有效IRI一起发送
* <a name="2.2.s3.b2"></a>由于类似的原因，语言映射的键必须与有效的 [RFC 5646](http://tools.ietf.org/html/rfc5646)语言标签一起发送。 
* <a name="2.2.s3.b3"></a>构造IRIs  SHOULD 使用库，而不是字符串连接 
* <a name="2.2.s3.b4"></a>变量SHOULD区分大小写除非特别申明
* <a name="2.2.s3.b5"></a>使用小写来发送不区分大小写的变量
* <a name="2.2.s3.b6"></a>除非本规范明确允许，否则SHOULD NOT将其他属性添加到语句中。 
* <a name="2.2.s3.b7"></a>属性不应在对象中多次出现。 如果属性在对象中多次使用，则LRS的行为是未定义的; 预期大多数LRS将使用他们现有的任何代码语言来完成解析JSON的功能。

__Note:__ 建议LRS 拒绝包含额外属性的语句，因为包含额外属性的语句可能不是LRS发送的

###### <a name="2.2.s4"></a>LRS Requirements 对LRS的要求

* <a name="2.2.s4.b1"></a>LRS 必须拒绝的语句
    * <a name="2.2.s4.b1.b1"></a>有任何空值的语句（在扩展里的除外）
    * <a name="2.2.s4.b1.b2"></a><a name="2.2.s4.b1.b3"></a>有着错误的数据类型，例如: 
        * 在数据类型为number的地方使用了string，尽管这个string是一个“number”或者
        * 在数据类型为booleans的地方使用了string，尽管这个string是一个“booleans”（string的2,string的true）
    * <a name="2.2.s4.b1.b4"></a>在需要特定格式的地方有任何没有依照格式的值，包括空string，有着特别格式的string（例如 mail-toIRI，UUID，或者IRI）
    * <a name="2.2.s4.b1.b5"></a>其中键的情况与本说明书中指定的情况不匹配。
    * <a name="2.2.s4.b1.b6"></a>其中限制枚举值的值的情况与本说明中给出的枚举值不匹配。
    * <a name="2.2.s4.b1.b7"></a>其中的键或者值在本说明中不被允许的。
    * <a name="2.2.s4.b1.b8"></a>包含了没有架构的IRL或者IRI。
* <a name="2.2.s4.b2"></a>LRS必须MUST至少验证语言映射密钥的令牌长度序列与[RFC 5646](http://tools.ietf.org/html/rfc5646)标准匹配.
* <a name="2.2.s4.b3"></a>LRS务必MUST处理和存储至少具有IEEE 754 32位浮点数精度的数字。
* <a name="2.2.s4.b4"></a>对于在语句中相同类型的值，LRS必须MUST按照相同的标准验证. __Note:__ 字符串参数值不像JSON中那样引用。
* <a name="2.2.s4.b5"></a>LRS 应该SHOULD对所有的值区分大小写，除非特别申明。
* <a name="2.2.s4.b6"></a>LRS 可MAY对IRL和IRI使用尽可能详细的验证，以满足不会被拒绝的要求。
* <a name="2.2.s4.b7"></a>LRS 可MAY对语言映射密匙使用尽可能详细的验证，以满足不会被拒绝的要求。
* <a name="2.2.s4.b8"></a>扩展的属性不应该SHOULD* NOT被添加到语句和其他对象中，除非本规范明确允许，并且LRS 应该SHOULD*拒绝包含这些附加属性的语句。

<a name="lifecycle" />

### <a name="2.3">2.3</a> Statement Lifecycle 语句的生态

语句是包含了跟踪学习活动的信息。通常这些语句中表示的信息已经发生，因此，在“display”或在“Verb ID”中人类可读部分中使用的自然语言使用过去时态。

语句被期望是永久性的，在本规范中撤销一个语句Statement的唯一方法是将他[无效化 void](#voided)，不是销毁该语句，而是表示这个语句被忽略。


<a name="statement-immutability-and-exceptions" />

#### <a name="2.3.1">2.3.1</a> Statement Immutability 语句不变性

语句是不能改变的，下面的说明是超出这条规则的情况:

* <a name="2.3.1.b1"></a>在LRS处理过程中，表示潜在和必须任务的属性（"id", "authority", "stored", "timestamp", "version"）。

* <a name="2.3.1.b2"></a>语句中引用的活动Activity定义，语句中引用的活动Activity定义的内容不被视为语句本身的一部分，这就意味着如果被引用的活动Activity定义的更改，则语句到JSON的深度序列化将改变。（详见 语句资源的“format”参数[Statement Resource's](./xAPI-Communication.md#stmtres)） 

* <a name="2.3.1.b3"></a>语句中引用的Verbs，Verb的“display”属性不被视为语句本身的一部分（详见 语句资源的“format”参数 [Statement Resource's](./xAPI-Communication.md#stmtres)）

* <a name="2.3.1.b4"></a>时间戳的序列化数据，这个本身就不被视为语句不变性的一部分。例如，只要参考的时间点本身不受影响，“timestamp”，和“stored”属性可以返回到存储它们的不同的时区的时间。
详见 [2.4.7 Timestamp](#timestamp) 和[2.4.8 Stored](#stored)。


* <a name="2.3.1.b5"></a>无序列表的序列化数据，组Group中的代理Agents列表不被认为是有序列表。因此，LRS可以以任何顺序返回该代理列表，详见 [Groups](#group)。

* <a name="2.3.1.b6"></a>附件，附件不是语句的一部分，当客户端请求它们时，LRS将返回没有附件的语句。
（详见 语句资源的“attachments”参数 [Statement Resource's](./xAPI-Communication.md#stmtres)）

* <a name="2.3.1.b7"></a>大小写区分，一些不区分大小写属性的大小写改变将不被视为影响不变性。例如，域名部分的电子邮件地址就不区分大小写。对于任何不区分大小写的文本，建议使用小写。

以下明确地不为例外，包含于该规则内。:

* <a name="2.3.1.b8"></a>Result Duration 由于年，月，甚至是分钟本身时间长短的不确定性，再加上代表着Activity开始，中间，结束的“timestamp”属性本身的可变性，让LRS来精确的解析Result Duration并且相互转换是不可能的。所以为了方便Result Duration的比较，采用string来表示。

<a name="statement-comparison-requirements" />
###### <a name="2.3.1.s9"></a>Statement Comparision Requirements 语句对比要求 
在本规范中概述了许多情况，需要比较语句以查看它们是否匹配。在这些情况下，以下规则适用:

* <a name="2.3.1.s9.b1"></a>由语句不变性的例外[exceptions to Statement immutability](#statement-immutability-and-exceptions)所引起的不同必须MUST被忽略。

* <a name="2.3.1.s9.b2"></a>对于任何属性序列化数据的不同且没有被列出在不变性例外[listed as exceptions](#statement-immutability-and-exceptions)中的必须不MUST NOT 被忽略。

<a name="voided"/>

#### <a name="2.3.2">2.3.2</a> Voiding 无效化，废止

###### <a name="2.3.2.s1"></a>Rationale 缘由

一个LRS能精确和完整地进行数据的收集是由语句不能被改变或者删除来保证的，语句的不变性是实现Experience API的分布式性质的关键因素。

然而，不是所有的语句一经生成，都将永久有效。错误或者其他因素都可能让先前的语句被标记为无效，这称为“无效语句”，内置Verb： `http://adlnet.gov/expapi/verbs/voided` 用于此目的。任何使另一个语句无效化的语句本身不能被无效。

###### <a name="2.3.2.s2"></a>Requirements 要求

* <a name="2.3.2.s2.b1"></a>当生成一个语句来无效化另外一个时，这个使无效语句的对象必须MUST包含设置为`StatementRef`的“objectType”属性。
* <a name="2.3.2.s2.b2"></a>当生成一个语句来无效化另外一个时，这个使无效语句的对象必须MUST申明需要被无效化语句的ID，这个ID就是该被无效化语句的“id”属性。
* <a name="2.3.2.s2.b3"></a>LRS 只能MUST在当且仅当这个语句本身不是一个使无效化语句时才能将一个语句考虑为无效的语句。并且LRS也需要把一个使无效化语句指向被无效化的语句。
* <a name="2.3.2.s2.b4"></a>当收到一个无效另一个语句的语句，如果请求不是从授权的void语句，LRS应该SHOULD拒绝包括无效语句的整个请求，使用403禁止`403 Forbidden`。
* <a name="2.3.2.s2.b5"></a>当收到一份声明使另一个声明失效时，LRS不应该SHOULD NOT*基于该声明的对象不存在而拒绝该声明。
* <a name="2.3.2.s2.b6"></a>当收到一个声明使另一个无效时，LRS可能需要MAY撤销对由刚刚失效的语句引入的活动或代理定义的任何更改。
* <a name="2.3.2.s2.b7"></a>一个学习记录提供者，想要对某个之前被无效化的语句进行“撤销无效化”的，应该SHOULD再次生成一个有着新ID的该语句。

__Note:__ 关于如何使一个语句与另一个相引用，参见于“当对象是语句时[When the "Object" is a Statement](#stmtasobj)”中的“语句引用["Statement References"](#stmtref)”， 关于当请求无效的语句，该语句是如何反馈的，详见第三部分的[StatementRef](./xAPI-Communication.md#queryStatementRef)。

###### <a name="2.3.2.s3"></a>Example 示例

这是一个展示语句无效化之前ID为"e05aa883-acaf-40ad-bf54-02c8ce485fb0"的语句的例子

```
{
	"actor" : {
		"objectType": "Agent",
		"name" : "Example Admin",
		"mbox" : "mailto:admin@example.adlnet.gov"
	},
	"verb" : {
		"id":"http://adlnet.gov/expapi/verbs/voided",
		"display":{
			"en-US":"voided"
		}
	},
	"object" : {
		"objectType":"StatementRef",
		"id" : "e05aa883-acaf-40ad-bf54-02c8ce485fb0"
	}
}
```  
<a name="statement-properties"/> 
### <a name="2.4">2.4</a> Statement Properties  语句属性

###### <a name="2.4.s1"></a>Details 详情
语句中每个属性的的详情被描述如下：

<table>
	<tr><th>Property</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.4.s1.table1.row1"><td>id</td><td>UUID</td>
	<td>UUID assigned by LRS if not set by the Learning Record Provider.<br>如果学习记录提供者没有设置的化由LRS来设置的UUID</td>
	<td>Recommended</td></tr>
	<tr id="2.4.s1.table1.row2"><td><a href="#actor">actor</a></td><td>Object</td>
	<td>Whom the Statement is about, as an <a href="#agent">Agent</a> or 
		<a href=#group>Group</a> Object.<br>这个语句的关于对象，可能是一个代理<a href="#agent">Agent</a>对象，或者是一个群体<a href=#group>Group</a>对象。</td>
	<td>Required</td></tr>
	<tr id="2.4.s1.table1.row3"><td><a href="#verb">verb</a></td><td>Object</td>
	<td>Action taken by the Actor. Actor<br>执行的动作</td>
	<td>Required</td></tr>
	<tr id="2.4.s1.table1.row4"><td><a href="#object">object</a></td><td>Object</td>
	<td>Activity, Agent, or another Statement that is the Object of the Statement.<br> 作为语句（动作）的对象（宾语），活动，代理或者另一个语句 
	</td>
	<td>Required</td></tr>
	<tr id="2.4.s1.table1.row5"><td><a href="#result">result</a></td><td>Object</td>
	<td>Result Object, further details representing a measured outcome.<br> 结果（成绩）对象，对于成绩的详细信息</td>
	<td>Optional</td></tr>
	<tr id="2.4.s1.table1.row6"><td><a href="#context">context</a></td><td>Object</td>
	<td>Context that gives the Statement more meaning. Examples: a team the Actor is 
	working with, altitude at which a scenario was attempted in a flight simulator.<br> 赋予语句更多意义的上下文。示例：和Actor一起工作的团队，在飞行模拟器场景中尝试的高度。</td>
	<td>Optional</td></tr>
	<tr id="2.4.s1.table1.row7"><td><a href="#timestamp">timestamp</a></td><td><a href="#timestamps">Timestamp</a></td>
	<td>Timestamp of when the events described within this Statement occurred. Set by the LRS if not provided.<br> 该语句所包含被描述事件发生的时间点，如果未设置的话，由LRS来设置。</td>
	<td>Optional</td></tr>
	<tr id="2.4.s1.table1.row8"><td><a href="#stored">stored</a></td><td><a href="#timestamps">Timestamp</a></td>
	<td>Timestamp of when this Statement was recorded. Set by LRS.<br> 语句被记录下来的时间，由LRS来设置</td>
	<td>Set by LRS</td></tr>
	<tr id="2.4.s1.table1.row9"><td><a href="#authority">authority</a></td><td>Object</td>
	<td>Agent or Group who is asserting this Statement is true. Verified by the LRS based on 
	authentication. Set by LRS if not provided or if a strong trust relationship between the Learning Record Provider 
	and LRS has not been established. <br>代理人或集团说明本声明是真实的，LRS基于身份的验证，如果没有提供，或者学习记录提供者和LRS之前没有建立牢固的信任关系，则由LRS设置</td>
	<td>Optional</td></tr>
	<tr id="2.4.s1.table1.row10"><td><a href="#version">version</a></td><td>Version</td>
	<td>The Statement’s associated xAPI version, formatted according to <a href="http://semver.org/spec/v1.0.0.html">Semantic Versioning 1.0.0</a>.<br> 语句所符合的xAPI版本，根据 <a href="http://semver.org/spec/v1.0.0.html">Semantic Versioning 1.0.0</a>来设置</td>
	<td>Not Recommended</td></tr>
	<tr id="2.4.s1.table1.row11">
		<td><a href="#attachments">attachments</a></td>
		<td>Ordered array of Attachment Objects</td>
	    <td>Headers for Attachments to the Statement 语句附件的标题</td>
	<td>Optional</td></tr>
</table>

###### <a name="2.4.s2"></a>Example

最简单的使用了所有必须或应该使用的属性的语句的示例。建议在具体情况下补充可选属性。当本语句从LRS返回时，它将包括由LRS添加的一些附加属性。
```
{
    "id": "12345678-1234-5678-1234-567812345678",
    "actor":{
        "mbox":"mailto:xapi@adlnet.gov"
    },
    "verb":{
        "id":"http://adlnet.gov/expapi/verbs/created",
        "display":{
            "en-US":"created"
        }
    },
    "object":{
        "id":"http://example.adlnet.gov/xapi/example/activity"
    }
}
```  
See [Appendix A: Example Statements](#Appendix2A) for more examples.更多示例参见附录A 

<a name="stmtid"/> 

#### <a name="2.4.1">2.4.1</a> ID 

###### <a name="2.4.1.s1"></a>Description 描述

一个UUID，[RFC 4122](http://www.ietf.org/rfc/rfc4122.txt)中变体2的所有版本都有效，并且UUID必须是标准字符串形式。

###### <a name="2.4.1.s2"></a>Requirements 要求

* <a name="2.4.1.s2.b1"></a>如果接受到的语句没有一个ID，那么LRS 必须 MUST 为其生成一个。
* <a name="2.4.1.s2.b2"></a>语句ID应当SHOULD由LRP来提供。

<a name="actor"/>

#### <a name="2.4.2">2.4.2</a> Actor  执行者，当事人

###### <a name="2.4.2.s1"></a>Description 描述
Actor定义了是谁来执行该动作的，Actor可以是一个代理Acgent或者一个群组Group 

<a name="agent"/>

##### <a name="2.4.2.1">2.4.2.1</a> When the Actor objectType is Agent 当Actor是Agent时
###### <a name="2.4.2.1.s1"></a>Description 描述
一个Agent是一个（单独的）人或者一个系统。

###### <a name="2.4.2.1.s2"></a>Details 详情

* <a name="2.4.2.1.s2.b1"></a>一个Agent 必须MUST是4种反函数标识符中的一个（见 [4.1.2.3 Inverse Functional Identifier 反函数标识符](#inversefunctional)）
* <a name="2.4.2.1.s2.b2"></a>一个Agent必须不能MUST NOT包括超过一个反函数标识符。
* <a name="2.4.2.1.s2.b3"></a>一个Agent不应当SHOULD NOT 使用在Group标识中也使用的反函数标识符。

下面这个表格列出了Agent Object的属性。

<table border ="1">
	<tr><th>Property</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.4.2.1.s2.table1.row1"><td>objectType</td><td>string</td><td><code>Agent</code>. This property is optional except when the Agent is used as a Statement's object.<br> 这个属性是可选的，除了在Agent Object作为语句的对象（宾语）时。</td>
	<td>Optional</td></tr>
	<tr id="2.4.2.1.s2.table1.row2"><td>name</td><td>String</td><td>Full name of the Agent. <br>代理的全名</td>
	<td>Optional</td></tr>
	<tr id="2.4.2.1.s2.table1.row3"><td colspan="2">see <a href="#inversefunctional"> 4.1.2.3 Inverse Functional Identifier</a></td>
	    <td>An Inverse Functional Identifier unique to the Agent.<br>一个与代理唯一对应的反函数标识符</td>
	    <td>Required</td></tr>
</table>


<a name="group"/>

##### <a name="2.4.2.2">2.4.2.2</a> When the Actor ObjectType is Group 当Actor是Group时
###### <a name="2.4.2.2.s1"></a>Description 描述

一个Group代表了多个Agents的集合，并且能在可以使用Agent的大多数的相同情况下使用。由两种类型的group：Anonymous匿名 Groups and Identified已标识 Groups组成.

###### <a name="2.4.2.2.s2"></a>Details 详情

一个匿名group是用来描述一组人，而这个group没有预先标识，例如 一个特设小组。

下面这个表列出了匿名group的属性。

<table border ="1">
	<tr><th>Property</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.4.2.2.s2.table1.row1"><td>objectType</td><td>String</td><td><code>Group</code>. </td><td>Required</td></tr>
	<tr id="2.4.2.2.s2.table1.row2"><td>name</td><td>String</td><td>Name of the Group.<br> 群组的名字</td><td>Optional</td></tr>
	<tr id="2.4.2.2.s2.table1.row3"><td>member</td><td>Array of <a href="#agent">Agent Objects</a></td>
	<td>The members of this Group. This is an unordered list.<br> Group的成员，无序列表</td>
	<td>Required</td></tr>
</table>

一个已标识Group是用来表示唯一身份的一组人

下面这个表列出了已标识group的属性

<table border ="1">
	<tr><th>Property</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.4.2.2.s2.table2.row1"><td>objectType</td><td>String</td><td><code>Group</code>. </td><td>Required</td></tr>
	<tr id="2.4.2.2.s2.table2.row2"><td>name</td><td>String</td><td>Name of the Group.<br>群组的名字</td><td>Optional</td></tr>
	<tr id="2.4.2.2.s2.table2.row3"><td>member</td><td>Array of <a href="#agent">Agent Objects</a></td>
	<td>The members of this Group. This is an unordered list.<br> Group的成员，无序列表</td>
	<td>Optional</td></tr>
	<tr id="2.4.2.2.s2.table2.row4"><td colspan="2">see <a href="#inversefunctional"> 4.1.2.3 Inverse Functional Identifier</a></td>
	    <td>An Inverse Functional Identifier unique to the Group. <br>一个与群组唯一对应的反函数标识符</td><td>Required</td></tr>	
</table>

###### <a name="2.4.2.2.s3"></a>Requirements 要求

* <a name="2.4.2.2.s3.b1"></a>一个学习记录消费者必须MUST将每个匿名的group视为一个特别的group，即使他们中可能有一些已标识的组员
* <a name="2.4.2.2.s3.b2"></a>当对一个group想发出多条语句，汇总数据和检索相关文件，一个学习记录提供者应该SHOULD使用已标识Group。
* <a name="2.4.2.2.s3.b3"></a>对于任何匿名或者已标识的Group，一个学习记录提供者 可MAY在“member”属性中提供部分或者完整的Agents 列表。
* <a name="2.4.2.2.s3.b4"></a>对于LRS返回的语句，Group member的列表可以依照任何顺序来排列。

###### <a name="2.4.2.2.s4"></a>Requirements for Anonymous Groups 对于匿名Group的要求

* <a name="2.4.2.2.s4.b1"></a>一个匿名的Group 必须MUST 包含一个“member”属性来列出组员Agents。
* <a name="2.4.2.2.s4.b2"></a>一个匿名的Group在其“member”标示中不能MUST NOT 包含一个Group 对象。

###### <a name="2.4.2.2.s5"></a>Requirements for Identified Groups 对于已标识Group的要求

* <a name="2.4.2.2.s5.b1"></a>一个已标识Group只能MUST包含一个反向函数标识符。
* <a name="2.4.2.2.s5.b2"></a>一个已标识Group在其“member”标示中不能MUST NOT 包含一个Group 对象。
* <a name="2.4.2.2.s5.b3"></a>一个已标识Group的反向函数标识符不应SHOULD NOT使用一个Agent也使用的身份标识。
* <a name="2.4.2.2.s5.b4"></a>一个已标识Group 可以MAY 包含一个“member”属性来列出组员Agents。

<a name="inversefunctional">

##### <a name="2.4.2.3">2.4.2.3</a> Inverse Functional Identifier 反向身份标识符
###### <a name="2.4.2.3.s1"></a>Description 描述
一个反向身份标识符 Inverse Functional Identifier (IFI)是用来标识唯一一个Agent 或者一个Group的一个值。

###### <a name="2.4.2.3.s2"></a>Rationale 缘由
为了使对某个Agents或Group进行相关的数据储存和检索，需要对其身份进行唯一标识。在xAPI语句中，我们使用以被广泛接受的FOAF原则推荐的反向身份标识符来完成（详见[Friend Of A Friend](http://xmlns.com/foaf/spec/#term_Agent)

###### <a name="2.4.2.3.s3"></a>Details 详情

下面这个表列出了所有反向身份标识符的可能属性。

<table border ="1">
	<tr><th>Property</th><th>Type</th><th>Description</th></tr>
	<tr id="2.4.2.3.s3.table1.row1"><td><a href="http://xmlns.com/foaf/spec/#term_mbox">mbox</a></td><td>mailto IRI</td><td>The required format is "mailto:email address".  格式为“mailto:email address” <br>
	Only email addresses that have only ever been and will ever be assigned to this Agent, 
but no others, SHOULD be used for this property and mbox_sha1sum.<br> 对于本属性和“mbox_sha1sum”属性，应当SHOULD使用只有对于某Agent的相关email地址。</td></tr>
	<tr id="2.4.2.3.s3.table1.row2"><td><a href="http://xmlns.com/foaf/spec/#term_mbox_sha1sum">mbox_sha1sum</a></td><td>String</td><td>The hex-encoded SHA1 hash of a mailto IRI (i.e. the value of an mbox property). An LRS MAY include Agents with a matching hash when a request is based on an mbox.<br> 对于mailto IRI的SHA1加密，一个LRS 可能MAY会包含相应的加密，当查询是以mbox作为基础时。</td></tr>
	<tr id="2.4.2.3.s3.table1.row3"><td>openid</td><td>URI</td><td>An openID that uniquely identifies the Agent. 一个唯一标识Agent的openID</td></tr>
	<tr id="2.4.2.3.s3.table1.row4"><td>account</td><td><a href="#agentaccount">Object</a></td><td>A user account on an existing system e.g. an LMS or intranet.<br> 一个存在于系统中的账户，例如一个LMS系统或者一个内网系统</td></tr>	
</table>

###### <a name="2.4.2.3.s4"></a>Client Requirements 对于客户的要求
* <a name="2.4.2.3.s4.b1"></a>电子邮件地址的域名部分是不区分大小写的。计算”mbox_sha1sum”属性的加密串时，客户端应该使用小写。

<a name="agentaccount"/>

##### <a name="2.4.2.4">2.4.2.4</a> Account Object 账户对象

###### <a name="2.4.2.4.s1"></a>Description 描述

一个存在于系统中的账户，例如一个LMS系统，一个内网系统或者一个公网系统

###### <a name="2.4.2.4.s2"></a>Details 详情

* <a name="2.4.2.4.s2.b1"></a>如果一个系统提供了一个使用了OpenID的account对象，那么学习记录提供者SHOULD 使用opendid属性，而不是一个account对象。
* <a name="2.4.2.4.s2.b2"></a>如果学习记录服务提供商对Agent或Group的个人身份信息非常需要，也应该用不透明的帐户名（例如帐号）来识别一个人的所有语句，同时保持匿名。

下面这个表列出了所有Account对象的可能属性。

<table border ="1">
	<tr><th>Property</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.4.2.4.s2.table1.row1"><td>homePage</td><td>IRL</td><td>The canonical home page for the system the account is on. This is based on FOAF's accountServiceHomePage. <br>该账户系统的主页，基于FOAF的accountServiceHomePage</td>
	<td>Required</td></tr>
	<tr id="2.4.2.4.s2.table1.row2"><td>name</td><td>String</td><td>The unique id or name used to log in to this account. This is based on FOAF's accountName.<br> 唯一的用来登录的用户名，基于FOAF的accountName</td><td>Required</td></tr>
</table>


###### <a name="2.4.2.4.s3"></a>Example 示例

这示范了一个使用不透明account的Agent例子：

```
{
	"objectType": "Agent",
	"account": {
		"homePage": "http://www.example.com",
		"name": "1625378"
	}
}
``` 

<a name="verb"/>

#### <a name="2.4.3">2.4.3</a> Verb 动词

###### <a name="2.4.3.s1"></a>Description 描述

Verb定义了Actor与Activity之间的操作

###### <a name="2.4.3.s2"></a>Rationale 缘由

在xAPI语句中Verb描述了学习过程中执行的操作。xAPI不指定任何特定的动词。（废止Void除外，即[http://adlnet.gov/expapi/verbs/voided](#voided)），相反，它定义了如何创建verb，使得xAPI实践社区可以建立有意义的动词从而可以被任何人使用，即verb的现有定义列表是有限的，可能无法准确的描述和捕捉到一切可能的学习活动。


###### <a name="2.4.3.s3"></a>Details 详情

出现在语句中的Verbs对象包含了一个IRI和一组包含了多种语言或者方言的显示名，以提供人类可读的的便利。下面这个表列出了所有Verb对象的可能属性。

<table>
	<tr><th>Property</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.4.3.s3.table1.row1">
		<td>id</td>
		<td>IRI</td>
		<td>Corresponds to a Verb definition. Each Verb definition 
			corresponds to the meaning of a Verb, not the word. <br>与动词相对应的定义。每个动词的定义对应于一个动词，而不是词的含义。 
		</td>
		<td>Required</td>
	</tr>
	<tr id="2.4.3.s3.table1.row2">
		<td>display</td>
		<td><a href="#lang-map">Language Map</a></td>
		<td>The human readable representation of the 
			Verb in one or more languages. This does not have any impact on the 
			meaning of the Statement, but serves to give a human-readable 
			display of the meaning already determined by the chosen Verb. <br>一个或多个语言动词的人类可读的表示。这不会对语句的含义的任何影响，但提供给已经被选择的动词确定含义的人类可读显示。</td>
		<td>Recommended</td>
	</tr>
</table>

###### <a name="2.4.3.s4"></a>Verb Id Requirements Verb ID 的要求

* <a name="2.4.3.s4.b1"></a>系统读取语句必须MUST使用verb IRI来推断意义。
* <a name="2.4.3.s4.b2"></a>包含在id中的IRI 应该SHOULD包含人类可识别的部分以方便于他人来回顾原始语句时，能分辨可能有歧义的相似Verb。
* <a name="2.4.3.s4.b3"></a>单个Verb IRI不能MUST NOT 指代多个含义。

###### <a name="2.4.3.s5"></a>Verb Display Learning Record Provider Requirements 对于LRP学习记录提供者的要求

* <a name="2.4.3.s5.b1"></a>所有的语句应当SHOULD使用“display”属性。
* <a name="2.4.3.s5.b2"></a>“display”属性必须MUST被申明，当Verb IRI中已经定义了，以用来说明意义。

###### <a name="2.4.3.s6"></a>Verb Display LRS Requirements 对于LRS的要求

下面是对于LRS返回来的“display”属性的要求。

* <a name="2.4.3.s6.b1"></a>当使用<code>exact</code>格式的查询时，LRS 必须MUST返回“display”属性。
* <a name="2.4.3.s6.b2"></a>当使用<code>ids</code>格式查询时，LRS不应该SHOULD NOT*返回”display”属性。
* <a name="2.4.3.s6.b3"></a>当使用<code>canonical</code>格式查询时，LRS应该SHOULD*返回”display”属性。
* <a name="2.4.3.s6.b4"></a>LRS 可能需要根据查询所得到语句中的“display”属性来定义一个标准显示。“name”属性元数据的描述参见[3.2 Hosted Metadata](#miscmeta)或其他地方的Verb‘Display

###### <a name="2.4.3.s7"></a>Verb Display Learning Record Consumer Requirements 关于Verb Display对于学习记录消费者的要求

下面是对学习记录消费者对于”display” 属性使用的要求.

* <a name="2.4.3.s7.b1"></a>“display”属性必须不能MUST NOT被用来改变Verb的意思。
* <a name="2.4.3.s7.b2"></a>LRC不能MUST NOT 使用“display”属性来推测语句的意思。
* <a name="2.4.3.s7.b3"></a>LRC不能MUST NOT 以除了显示给人看的其他用意来使用“display”属性。
使用“display”属性来给语句分类就是一个违反要求的例子。
* <a name="2.4.3.s7.b4"></a>学习记录消费者在用户界面中显示语句动词可以MAY 选择使用语句中“display”属性的值。
* <a name="2.4.3.s7.b5"></a>学习记录消费者在显示语句中的Ver时，不能MUST NOT选择会导致verb意义改变的词。 

###### <a name="2.4.3.s8"></a>Example 示例
下面示范了一个使用推荐属性的verb，使用了美国英语US English和西班牙语Spanish 
```
{
    "id":"http://example.com/xapi/verbs#defenestrated", 
    "display":{
        "en-US":"defenestrated",
        "es" : "defenestrado" 
    } 
}
``` 
			
##### <a name="2.4.3.1">2.4.3.1</a> Use in Language and Semantics of Verbs 语义

###### <a name="2.4.3.1.s1"></a>Details 详细

_Semantics语义_

Verb所代表的IRI是对一个词语义的说明，而不是这个词本身。

例如，英语中的“fired”在不同语境中有不同的意思例如“开火”（对于武器），“烧”（火），“炒了”（员工）,在这个例子中，一个IRI标识着其中一个意义。

“display”属性在时态上有着的可变性。

_Language语言_

xAPI中的Verb IRI并不依赖于某种特定语言。

例如， http://example.org/firearms#fire 可能表示游戏中的开枪动作， http://example.com/فعل/خواندن 可能表示读了某本书。

<a name="object"/>

#### <a name="2.4.4">2.4.4</a> Object 对象（宾语）

###### <a name="2.4.4.s1"></a>Description 描述

对象用于定义被作用的活动，一个语句的对象可以是一个activity 也可以是一个Agent，一个Group，或者一个语句，或者语句参考。

Some examples:

* <a name="2.4.4.s1.b1"></a>The Object is an Activity: "Jeff wrote an essay about hiking."

* <a name="2.4.4.s1.b2"></a>The Object is an Agent: "Nellie interviewed Jeff."

* <a name="2.4.4.s1.b3"></a>The Object is a SubStatement or Statement Reference (different implementations, but similar 
when human-read): "Nellie commented on 'Jeff wrote an essay about hiking.'"

###### <a name="2.4.4.s2"></a>Details 详情

对于作为对象（宾语）的对象，应当SHOULD 包含于一个“objectType”属性，如果没有申明，那么objectType将被视为`Activity`，其他的有效值是：`Agent`，`Group`, `SubStatement` 或者 `StatementRef`。这个属性根据对象而改变。

<a name="activity"/>

##### <a name="2.4.4.1">2.4.4.1</a> When the ObjectType is Activity 当对象类型为活动时

###### <a name="2.4.4.1.s1"></a>Details 详情

一个语句能将activity作为对象（宾语），下表给出了这种情况的对象属性。

<table>
	<tr><th>Property</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.4.4.1.s1.table1.row1">
		<td>objectType</td>
		<td>String</td>
		<td>MUST be <code>Activity</code> when present<br> 必须为<code>Activity</code></td>
		<td>Optional</td>
	</tr>
	<tr id="2.4.4.1.s1.table1.row2">
		<td><a href="#acturi">id</a></td><td>IRI</td>
		<td>An identifier for a single unique Activity <br>对于一个活动的唯一标识</td>
		<td>Required</td>
	</tr>
	<tr id="2.4.4.1.s1.table1.row3">
		<td><a href="#actdef">definition</a></td>
		<td>Object</td>
		<td>Metadata <br>元数据, <a href="#actdef">See below 参见下文</a></td>
		<td>Optional</td>
	</tr>
</table>

如果对于两个不同的Activities可以使用同样的ID，那么就说明对于语句的验证出了问题，这意味着LRS不能将一个相同的ID去解析为两个不同的活动activities，虽然这有可能只是命名上的相同，但系统还是不能将其分别出来。


###### <a name="2.4.4.1.s2"></a><a name="actdef" />Activity Definition 定义活动
下表列出了activity definition object定义活动对象的属性：

<table>
	<tr><th>Property</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.4.4.1.s2.table1.row1">
		<td>name</td>
		<td><a href="#lang-maps">Language Map</a></td>
		<td>The human readable/visual name of the Activity<br> 人类可读的名字</td>
		<td>Recommended</td>
	</tr>
	<tr id="2.4.4.1.s2.table1.row2">
		<td>description</td>
		<td><a href="#lang-maps">Language Map</a></td>
		<td>A description of the Activity<br>描述</td>
		<td>Recommended</td>
	</tr>
	<tr id="2.4.4.1.s2.table1.row3">
		<a name="acttype"/>
		<td>type</td>
		<td>IRI</td>
		<td>The type of Activity.<br> 活动的类型</td>
		<td>Recommended</td>
	</tr>
	<tr id="2.4.4.1.s2.table1.row4">
		<td>moreInfo</td>
		<td>IRL</td>
		<td>Resolves to a document with human-readable information about the Activity, 
		which could include a way to launch the activity.<br>有关该活动更多信息的文档
		</td>
		<td>Optional</td>
	</tr>
	<tr>
		<td colspan="4">Interaction properties, See: <a href="#interactionacts">Interaction Activities</a> <br>交互属性，参见<a href="#interactionacts">Interaction Activities</a></td>
	</tr>
	<tr id="2.4.4.1.s2.table1.row5">
		<td>extensions</td>
		<td>Object</td>
		<td>A map of other properties as needed (see: <a href="#miscext">Extensions</a>)<br>一系列其他需要的属性，见<a href="#miscext">扩展Extensions</a></td>
		<td>Optional</td>
	</tr>
</table>

__Note:__ IRI片段（有时称为相对IRL）不是有效的IRI。与Verb一样，建议实现xAPI的人们查找和使用已建立的，广泛采用的活动类型。

 
###### <a name="2.4.4.1.s3"></a><a name="acturi" />Activity id Requirements 对 Activity Id的要求

* <a name="2.4.4.1.s3.b1"></a>一个Activity id 必须MUST唯一 
* <a name="2.4.4.1.s3.b2"></a>一个Activity id 必须MUST 指向同一Activity
* <a name="2.4.4.1.s3.b3"></a>一个Activity id 应当SHOULD使用被授权的域名.
* <a name="2.4.4.1.s3.b4"></a>一个Activity id 应当SHOULD根据一个情景方案来创建，并确保其中所以的id都保持唯一
* <a name="2.4.4.1.s3.b5"></a>一个Activity id 可MAY 指向该活动的元数据或者IRL

###### <a name="2.4.4.1.s4"></a>LRS Requirements 对LRS要求

* <a name="2.4.4.1.s4.b1"></a>LRS在其感知到多个作者和/或组织正在使用活动ID的情况下不得采取行动
* <a name="2.4.4.1.s4.b2"></a>LRS不得将对相同活动ID的引用视为对不同活动的引用。
* <a name="2.4.4.1.s4.b3"></a>在收到对某个活动具有不同定义的语句时，LRS应该决定它是否是LRP所授权的，如果是肯定的，那么就应该更新该活动的定义
* <a name="2.4.4.1.s4.b4"></a>LRS可以对其接收时的活动的规范定义进行小的修正。例如，新定义以固定拼写。
* <a name="2.4.4.1.s4.b5"></a>LRS不应对活动的规范定义进行重大更改。 例如基于更新的定义。更改正确的响应。


###### <a name="2.4.4.1.s5"></a>Learning Record Provider Requirements 对LRP的要求

* <a name="2.4.4.1.s5.b1"></a>一个LRP学习记录提供商必须MUST确保一个ID不能用于多种活动
* <a name="2.4.4.1.s5.b2"></a>一个LRP针对某一Activity ID 只能去生成与先前存储的同id相符的陈述或语句相同的陈述或语句。
* <a name="2.4.4.1.s5.b3"></a>一个LRP不能MUST NOT允许任何新版本破坏activity的兼容性

<a name="interactionacts"/>

##### <a name="2.4.4.1.s6"></a>Interaction Activities 交互活动

###### <a name="2.4.4.1.s7"></a>Rationale 缘由

传统的e-learning有包括互动或者评估的体系，为了使这些方法在xapi中扩展，这个规范借鉴了SCORM 2004的数据模型，从而定义了交互Interaction。对SCORM数据模型的直接引用已经开始废除了，任何相关的要求，都在本说明中直接包含了。

这些Interaction的定义是较为简单易用的，但也因此有限，对于实践社区，预期需要使用活动类型和活动定义扩展来达到更丰富的定义。

###### <a name="2.4.4.1.s8"></a>Details 详情

下表列出了交互活动Interaction Activities的属性

<table>
	<tr><th>Property</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.4.4.1.s8.table1.row1">
		<td>interactionType</td>
		<td>String</td>
		<td>The type of interaction. Possible values are: <code>true-false</code>, <code>choice</code>, <code>fill-in</code>, <code>long-fill-in</code>,
		<code>matching</code>, <code>performance</code>, <code>sequencing</code>, <code>likert</code>, <code>numeric</code> or <code>other</code>.<br> 交互的类型，可能的值为：<code>true-false</code>, <code>choice</code>, <code>fill-in</code>, <code>long-fill-in</code>,
		<code>matching</code>, <code>performance</code>, <code>sequencing</code>, <code>likert</code>, <code>numeric</code> or <code>other</code></td>
		<td>Required</td>
	</tr>
	<tr id="2.4.4.1.s8.table1.row2">
		<td>correctResponsesPattern</td>
		<td>Array of Strings</td>
		<td>A pattern representing the correct response to the interaction. The structure of this pattern varies
		depending on the interactionType. This is detailed below.<br>代表着交互活动Interaction Activities正确的响应参数，这个参数的结构取决于interactionType而变化。这将在下面详细说明。 </td>
		<td>Optional</td>
	</tr>
	<tr id="2.4.4.1.s8.table1.row3">
		<td>choices | scale | source | target | steps</td>
		<td>Array of interaction components</td>
		<td>Specific to the given interactionType (see below).<br>由给定的interactionType而决定的特性（参考后文）</td>
		<td>Optional</td>
	</tr>
</table>

###### <a name="2.4.4.1.s9"></a>Interaction Types 交互类型

下面的表描述了由每个interactionTypes所表示的各种Interaction。这些类型的相互作用最初用于基于SCORM 2004第4版运行环境的“cmi.interactions.n.type”参阅附录C[Appendix C](#Appendix2C)查看定义实例。 

<table>
	<tr><th>interactionType</th><th>Description</th></tr>
	<tr id="2.4.4.1.s9.table1.row1">
		<td>true-false</td>
		<td>An interaction with two possible responses: <code>true</code> or <code>false</code>.<br> 由两种响应结果的交互，<code>true</code> or <code>false</code> </td>
	</tr>
	<tr id="2.4.4.1.s9.table1.row2">
		<td>choice</td>
		<td>An interaction with a number of possible choices from which the learner can select. 
			This includes interactions in which the learner can select only one answer from the list and
			those where the learner can select multiple items.
			<br>学习者可以从许多可能的选择中进行选择的交互，包含了单项选择和多项选择。
		</td>
	</tr>
	<tr id="2.4.4.1.s9.table1.row3">
		<td>fill-in</td>
		<td>An interaction which requires the learner to supply a short response in the form of one or more 
			strings of characters. Typically, the correct response consists of part of a word, one word or a few words. 
			"Short" means that the correct responses pattern and learner response strings will normally be 250 characters or less.<br>学习者需要反馈一个短小的回答的交互，可能是某个词或者某几个词，“短小”意味着一般不超过250的字符。
		</td>
	</tr>
	<tr id="2.4.4.1.s9.table1.row4">
		<td>long-fill-in</td>
		<td>An interaction which requires the learner to supply a response in the form of a long string of characters.
			"Long" means that the correct responses pattern and learner response strings will normally be more than 250 characters.<br>学习者需要反馈一个长段的回答的交互，“长”以为这一般超过了250个字符
		</td>
	</tr>
	<tr id="2.4.4.1.s9.table1.row5">
		<td>matching</td>
		<td>An interaction where the learner is asked to match items in one set (the source set) to items in another set (the target set).
			Items do not have to pair off exactly and it is possible for multiple or zero source items to be matched to a given target and vice versa.
			<br>学习者需要对一系列设置好的语句或者概念进行匹配的交互。
			</td>
	</tr>
	<tr id="2.4.4.1.s9.table1.row6">
		<td>performance</td>
		<td>An interaction that requires the learner to perform a task that requires multiple steps.<br>学习者需要完成一个包含着多个步骤的任务的交互</td>
	</tr>
	<tr id="2.4.4.1.s9.table1.row7">
		<td>sequencing</td>
		<td>An interaction where the learner is asked to order items in a set.<br>学习者需要将一系列对象进行排序的交互</td>
	</tr>
	<tr id="2.4.4.1.s9.table1.row8">
		<td>likert</td>
		<td>An interaction which asks the learner to select from a discrete set of choices on a scale<br>学习者需要在一个离散阶梯中做出一个选择的交互（例如：1满意2一般，3不满意，4非常不满意）</td>
	</tr>
	<tr id="2.4.4.1.s9.table1.row9">
		<td>numeric</td>
		<td>Any interaction which requires a numeric response from the learner.<br>学习者需要返回一个数字的交互</td>
	</tr>
	<tr id="2.4.4.1.s9.table1.row10">
		<td>other</td>
		<td>Another type of interaction that does not fit into those defined above.<br>以上定义中未提到其他种类的交互</td>
	</tr>
</table>

###### <a name="2.4.4.1.s10"></a>Response Patterns 返回参数
The下面这个表给出了每个交互“correctResponsesPattern”属性字符串string的格式，这种格式也用于结果对象Result Object中的学习者响应。这些格式最初用于基于SCORM 2004第4版运行环境的“cmi.interactions.n.type”参阅附录C查看格式实例 [Appendix C](#Appendix2C) 


<table>
	<tr><th>interactionType</th><th>Format</th></tr>
	<tr id="2.4.4.1.s10.table1.row1">
		<td>true-false</td>
		<td>Either <code>true</code> or <code>false</code></td>
	</tr>
	<tr id="2.4.4.1.s10.table1.row2">
		<td>choice</td>
		<td>A list of item ids delimited by <code>[,]</code>. If the response contains only one item, the delimiter MUST not be used. <br>一系列被<code>[,]</code>分割的选项id。如果只有一个，那么就不使用分割符</td>
	</tr>
	<tr id="2.4.4.1.s10.table1.row3">
		<td>fill-in and long-fill-in</td>
		<td>A list of responses delimited by <code>[,]</code>. If the response contains only one item, the delimiter MUST not be used.<br>一系列被<code>[,]</code>分割的响应。如果只有一个，那么就不使用分割符</td>
	</tr>
	<tr id="2.4.4.1.s10.table1.row4">
		<td>matching</td>
		<td>A list of matching pairs, where each  pair consists of a source item id followed by a target item id. 
			Items can appear in multiple (or zero) pairs.
			Items within a pair are delimited by <code>[.]</code>. Pairs are delimited by <code>[,]</code>.
			
			<br>配对的列表，其中每对由源项的id后跟一个靶项的id，之间由<code>[.]</code>分割，对与对之间由<code>[,]</code>分割
		</td>
	</tr>
	<tr id="2.4.4.1.s10.table1.row5">
		<td>performance</td>
		<td>
			A list of steps containing a step ids and the response to that step.
			Step ids are separated from responses by <code>[.]</code>. Steps are delimited by <code>[,]</code>.
			The response can be a String as in a fill-in interaction or a number range as in a numeric interaction. 
			<br>步骤的列表，其中每对由步骤id后跟该步骤的响应，之间由<code>[.]</code>分割，对与对之间由<code>[,]</code>分割。
		</td>
	</tr>
	<tr id="2.4.4.1.s10.table1.row6">
		<td>sequencing</td>
		<td>An ordered list of item ids delimited by <code>[,]</code>.
		<br>一个排好序的项目id列表，由<code>[,]</code>分割</td>
	</tr>
	<tr id="2.4.4.1.s10.table1.row7">
		<td>likert</td>
		<td>A single item id<br>一个单独的选项ID</td>
	</tr>
	<tr id="2.4.4.1.s10.table1.row8">
		<td>numeric</td>
		<td>A range of numbers represented by a minimum and a maximum delimited by <code>[:]</code>. 
			Where the range does not have a maximum or does not have a minimum, that number is omitted but the delimiter is
			still used. E.g. <code>[:]4</code> indicates a maximum for 4 and no minimum. 
			Where the correct response or learner's response is a single number rather than a range, the single number
			with no delimiter MAY be used. 
			<br>一个单独的数字，或者如果是表示一个数字区间的话，由最小值和最大值加上分割符<code>[:]</code>组成，如果没有某个上限值，那么那个上限值被忽略，但是分隔符依然存在，例如<code>[:]</code>4表示最大值为4，没有最小值
		</td>
	</tr>
	<tr id="2.4.4.1.s10.table1.row9">
		<td>other</td>
		<td>Any format is valid within this string as appropriate for the type of interaction.<br>任何对于其他交互的有效合理的反馈格式</td>
	</tr>
</table>

###### <a name="2.4.4.1.s11"></a>Correct Responses Pattern 正确响应参数（参考答案）

TheCorrect Responses Pattern正确响应参数中包含着一个响应参数数组Array，一个学习者的响应如果和任何该参数数组里的值匹配的话，就会被视为正确，当一个响应参数本身又是一个分割开的列表时，只有当学习者的响应与这一个响应参数中的所有项都匹配时，才被视为正确。例如，假设正确响应参数为:

```
"correctResponsesPattern": [
    "foo[,]bar",
    "foo"
]
``` 

那么同时 foo和bar，或者单单只是foo都被视为正确，但是单单只是bar的话就不被视为正确

对于正确响应参数Correct Responses Pattern，一旦使用的话，应该尽可能的去保证建立所有正确响应的清单，但凡问题的正确标准是复杂的，学习记录提供商不被鼓励使用正确响应参数。

学习记录消费者通过对比响应与正确响应参数是不能被称之为成功的，更不能依赖正确响应参数是全面的，学习记录提供者是可以将不与正确响应参数相匹配的答案视为正确的，虽然这是不被鼓励的。

当正确响应参数包含一个空数组Array时，说明没有正确答案，而当任何答案都是正确的情况时，正确响应参数将被忽略。

###### <a name="2.4.4.1.s12"></a>Characterstring parameters

上面所描述的一些响应的值可以被预扩展某些参数，这些参数由格式`{parameter=value}`表示，这最初基于SCORM 2004第4版运行环境的字符串分割来定义的，参阅附录C [the long-fill-in example within Appendix C](#long-fill-in)查看简答题实例。

字符串参数是不由LRS来做验证的，系统解读语句数据时能尽最大程度的解读或者忽略不合法的字符串参数和值。

下列参数在列出的交互类型中放置在开头来代表对应的对应项，是有效的。
<table>
	<tr><th>Parameter</th><th>Default</th><th>Description</th><th>Value</th><th>Interaction types</th></tr>
	<tr id="2.4.4.1.s12.table1.row1">
		<td>case_matters</td>
		<td>false</td>
		<td>Whether or not the case of items in the list matters. <br>是否区分大小写</td>
		<td><code>true</code> or <code>false</code></td>
		<td>fill-in, long-fill-in</td>
	</tr>
	<tr id="2.4.4.1.s12.table1.row2">
		<td>order_matters</td>
		<td>true</td>
		<td>Whether or not the order of items in the list matters. <br>是否有序无序或者无序的列表有影响</td>
		<td><code>true</code> or <code>false</code></td>
		<td>fill-in, long-fill-in, performance</td>
	</tr>
</table>

下面的参数在列出的交互类型中在每一项的开头放置时有效的：
<table>
	<tr><th>Parameter</th><th>Description</th><th>Value</th><th>Interaction types</th></tr>
	<tr id="2.4.4.1.s12.table2.row1">
		<td>lang</td>
		<td>The language used within the item. <br>对于该项使用的语言</td>
		<td><a href="http://tools.ietf.org/html/rfc5646">RFC 5646 Language Tag</a></td>
		<td>fill-in, long-fill-in, performance (String responses only)</td>
	</tr>
</table>


###### <a name="2.4.4.1.s13"></a>Requirements 要求

* <a name="2.4.4.1.s13.b1"></a>Interaction Activities交互活动 必须MUST有一个有效的 交互类型interactionType
* <a name="2.4.4.1.s13.b2"></a>Interaction Activities应该SHOULD 有活动类型 
`http://adlnet.gov/expapi/activities/cmi.interaction`.
* <a name="2.4.4.1.s13.b3"></a>一个LRS，在验证有了一个有效的交互类型interactionType之后，可能MAY需要验证剩下的属性，可能MAY回被返回`400 Bad Request`，如果剩下的属性没有通过验证的话。 
* <a name="2.4.4.1.s13.b4"></a>LRS 不应当SHOULD* NOT 强制限制响应的字符数量
* <a name="2.4.4.1.s13.b5"></a>LRS 不应当SHOULD* NOT限制正确响应参数Correct Responses Pattern数组的长度


##### <a name="2.4.4.1.s14"></a>Interaction Components 交互组件

###### <a name="2.4.4.1.s15"></a>Details 详情

交互组件定义如下： 

<table>
	<tr><th>Property</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.4.4.1.s15.table1.row1">
		<td>id</td>
		<td>String</td>
		<td>Identifies the interaction component within the list.<br>标识交互组件到到一个列表</td>
        <td>Required</td>
	<tr>
		<td>description</td>
		<td><a href="#lang-maps">Language Map</a></td>
		<td>A description of the interaction component 
			(for example, the text for a given choice in a multiple-choice interaction)<br>对于交互组件的描述（例如对于给定多项选择的段落）</td>
		<td>Optional</td>
	</tr>
</table>

<a name="#interactionComponentLists"/>

取决于交互类型，交互活动能附加属性，每一个都包含一个交互组件列表，这些附加属性被称为交互组件表"interaction component lists"，下表展示了对于相应交互类型支持的交互组件列表。

<table>
	<tr id="2.4.4.1.s15.table2.row1"><th>interactionType</th><th>supported interaction component list(s)</th><th>Description</th><tr>
	<tr><td>choice, sequencing</td><td>choices</td>
	<td>A list of the options available in the interaction for selection or ordering.<br>一个选项的列表</td></tr>
	<tr id="2.4.4.1.s15.table2.row2"><td>likert</td><td>scale</td>
	<td>A list of the options on the likert scale.<br>一个表示不同程度的离散阶梯。</td></tr>
	<tr id="2.4.4.1.s15.table2.row3"><td>matching</td><td>source, target</td>
	<td>Lists of sources and targets to be matched.<br>源项和靶项的列表</td></tr>
	<tr id="2.4.4.1.s15.table2.row4"><td>performance</td><td>steps</td>
	<td>A list of the elements making up the performance interaction.<br>performance交互的元素的列表</td></tr>
	<tr id="2.4.4.1.s15.table2.row5"><td>true-false, fill-in, long-fill-in, numeric, other</td><td>[No component lists supported]</td><td></td></tr>
</table>


###### <a name="2.4.4.1.s16"></a>Requirements 要求

* <a name="2.4.4.1.s16.b1"></a>对于交互组件的数组，所有的id值必须MIUST是不同的
* <a name="2.4.4.1.s16.b2"></a>一个交互组件的id不应当SHOULD NOT包含空格（空白）

###### <a name="2.4.4.1.s17"></a>Examples 例子

参阅附录C [Appendix C](#Appendix2C) 

<a name="agentasobj"/>

##### <a name="2.4.4.2">2.4.4.2</a> When the "Object" is an Agent or a Group 当object为Agent或者Group

###### <a name="2.4.4.2.s1"></a>Requirements 要求

* <a name="2.4.4.2.s1.b1"></a>将Agent或者Group作为为Object（宾语）时，必须申明"objectType"属性

详见[Actor](#actor)中的Agent。 

<a name="stmtasobj"/>

##### <a name="2.4.4.3">2.4.4.3</a> When the "Object" is a Statement 当object为语句Statement时

###### <a name="2.4.4.3.s1"></a>Rationale

这里有两种情况会用到将语句Statement作为Object，1，一个对象利用已经使用过的语句的形式而运用语句引用Statement Reference，一个对于语句引用的常见的例子就是评论或分类一个学习活动，而这又作为一个单独的事件。无效化某语句的特例也使用了语句引用Statement Reference。2，一个对象能够通过使用字语句组成一个新的语句。每一种类型定义入下。

<a name="stmtref"/>

##### <a name="2.4.4.3.s2"></a>Statement References 语句引用

###### <a name="2.4.4.3.s3"></a>Description 描述
一个对于已经存在的语句的引用。

###### <a name="2.4.4.3.s4"></a>Requirements 要求

* <a name="2.4.4.3.s4.b1"></a>一个语句引用Statement Reference 必须MUST 申明"objectType" 属性为 `StatementRef`.
* <a name="2.4.4.3.s4.b2"></a>一个语句引用Statement Reference 必须MUST将语句的UUID设置到“id”属性。且LRS不用再次对已经存在语句的UUID进行验证。

下表列出了语句引用Statement reference对象的所有属性：

<table border ="1">
	<tr><th>Property</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.4.4.3.s4.table1.row1"><td>objectType</td><td>String</td><td>In this case, MUST be <code>StatementRef</code>.<br>在这里必须为<code>StatementRef</code>.</td><td>Required</td></tr>
	<tr id="2.4.4.3.s4.table1.row2"><td>id</td><td>UUID</td><td>The UUID of a Statement. <br> 一个语句的UUID
	</td><td>Required</td></tr>
</table>

###### <a name="2.4.4.3.s5"></a>Example 示例

假设一个语句已经已经被以ID为`8f87ccde-bb56-4c2e-ab83-44982ef22df0`而储存了，下面示范了如何实现使用一个新的语句来评论它

```
{
	"actor" : { 
		"objectType": "Agent", 
		"mbox":"mailto:test@example.com" 
	},
	"verb" : { 
		"id":"http://example.com/commented", 
		"display": {
			"en-US":"commented"
		} 
	},
	"object" : {
		"objectType":"StatementRef",
		"id":"8f87ccde-bb56-4c2e-ab83-44982ef22df0"
	},
	"result" : { 
		"response" : "Wow, nice work!" 
	}
}
``` 

<a name="substmt"/>

##### <a name="2.4.4.3.s6"></a>SubStatements 子语句

###### <a name="2.4.4.3.s7"></a>Description 描述
一个子语句就像一个语句引用StatementRef一样，用来作为某个语句的一部分，但是区别是，不同于StatementRef，子语句不表示一个新的事件的发生。可用来描述，例如，对某个潜在的未来的语句的预测或者一个老师评价一个学生时（这并不算做学生的行为）。

###### <a name="2.4.4.3.s8"></a>Requirements 要求

* <a name="2.4.4.3.s8.b1"></a>一个子语句SubStatement 必须 MUST申明"objectType" 属性为 `SubStatement`.
* <a name="2.4.4.3.s8.b2"></a>一个子语句SubStatement 必须 MUST被作为一个语句来验证
* <a name="2.4.4.3.s8.b3"></a>一个子语句SubStatement 不能 MUST NOT包含"id", "stored", "version" 或者 "authority"属性
* <a name="2.4.4.3.s8.b4"></a>一个子语句SubStatement不能 MUST NOT包含其自己的子语句，即不能嵌套。

###### <a name="2.4.4.3.s9"></a>Example 示例

一个有趣的使用子语句SubStatements的例子是在创建意向语句时，例如，使用子语句我们可以创建形式为`"<I> <planned> (<I> <did> <this>)"`的语句来表达我们计划将要做某事，一个具体的遵循逻辑的例子展示如下，“我计划访问一些很酷的网站”。
 


```
{
	"actor": {
		"objectType": "Agent", 
		"mbox":"mailto:test@example.com" 
	},
	"verb" : { 
		"id":"http://example.com/planned", 
		"display":{
			"en-US":"planned"
		} 
	},
	"object": {
		"objectType": "SubStatement",
		"actor" : {
			"objectType": "Agent", 
			"mbox":"mailto:test@example.com" 
		},
		"verb" : { 
			"id":"http://example.com/visited", 
			"display":{
				"en-US":"will visit"
			} 
		},
		"object": {
			"objectType": "Activity",
			"id":"http://example.com/website",
			"definition": { 
				"name" : {
					"en-US":"Some Awesome Website"
				}
			}
		}
	}
}
```

<a name="result"/>

#### <a name="2.4.5">2.4.5</a> Result Result 对象

###### <a name="2.4.5.s1"></a>Description 描述

一个可选属性，代表着相应语句的结果

###### <a name="2.4.5.s2"></a>Details

下表包含了结果对象的属性

<table border="1">
<tr><th>Property</th><th>Type</th><th>Description</th><th>Required</th></tr>
<tr id="2.4.5.s2.table1.row1">
	<td>score</td>
	<td>Object</td>
	<td>The score of the Agent in relation to the success or quality of the experience. <br>一个与成功或者质量相关的得分。<br>
	<a href ="#Score">See: Score</a></td>
	<td>Optional</td>
</tr>
<tr id="2.4.5.s2.table1.row2">
	<td>success</td>
	<td>Boolean</td>
	<td>Indicates whether or not the attempt on the Activity was successful.<br>表示是否成功</td>
	<td>Optional</td>
</tr>
<tr id="2.4.5.s2.table1.row3">
	<td>completion</td>
	<td>Boolean</td>
	<td>Indicates whether or not the Activity was completed.<br>表示是否完成</td>
	<td>Optional</td>
</tr>
<tr id="2.4.5.s2.table1.row4">
	<td>response</td>
	<td>String</td>
	<td>A response appropriately formatted for the given Activity.<br>对给定活动的有着合理格式的反馈（响应）</td>
	<td>Optional</td>
</tr>
<tr id="2.4.5.s2.table1.row5">
	<td>duration</td>
	<td><a href="#durations">Duration</a></td>
	<td>Period of time over which the Statement occurred.<br>语句发生的时间长度</td>
	<td>Optional</td>
</tr>
<tr id="2.4.5.s2.table1.row6">
	<td>extensions</td>
	<td>Object</td>
	<td>A map of other properties as needed.<br>需要的其他属性的结构<br>
	<a href="#miscext">See: Extensions</a></td>
	<td>Optional</td>
</tr>
</table>

<a name="Score"/>

##### <a name="2.4.5.1">2.4.5.1</a> Score 得分
 
###### <a name="2.4.5.1.s1"></a>Description 描述
一个代表着学习者达成分数的可选属性

###### <a name="2.4.5.1.s2"></a>Details 详情

Score对象定义如下表

<table border ="1">
	<tr><th>Property</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.4.5.1.s2.table1.row1">
		<td>scaled</td>
		<td>Decimal number between -1 and 1, inclusive</td>
		<td>The score related to the experience as modified by scaling and/or normalization.<br>对于相关活动的缩放或归一化分数。
		</td>
		<td>Recommended</td>
	</tr>
	<tr id="2.4.5.1.s2.table1.row2">
		<td>raw</td>
		<td>Decimal number between min and max (if present, otherwise unrestricted), inclusive</td>
		<td>The score achieved by the Actor in the experience described by the Statement. This is not modified by
		any scaling or normalization.<br>对于相关活动的原始分数</td>
		<td>Optional</td>
	</tr>
	<tr id="2.4.5.1.s2.table1.row3">
		<td>min</td>
		<td>Decimal number less than max (if present)</td>
		<td>The lowest possible score for the experience described by the Statement.<br>相关活动的最少可能分数</td>
		<td>Optional</td>
	</tr>
	<tr id="2.4.5.1.s2.table1.row4">
		<td>max</td>
		<td>Decimal number greater than min (if present)</td>
		<td>The highest possible score for the experience described by the Statement.<br>相关活动的最多可能分数</td>
		<td>Optional</td>
	</tr>
</table>

Score 分数对象的属性是基于cmi。Score的相应属性，如SCORM 2004第四版限定。“scaled缩放”和”raw原始”属性不一定有直接联系，因为缩放和归一化是因不同学习记录提供者不同xAPI实践社区二不同的，分数的缩放和归一化在这里不做谈论。

###### <a name="2.4.5.1.s3"></a>Requirements 要求

* <a name="2.4.5.1.s3.b1"></a>分数对象Score Object 应该SHOULD 包含“scale”，如果能得出一个逻辑百分比的话。
* <a name="2.4.5.1.s3.b2"></a>分数对象Score Object 不应该SHOULD NOT用于评估完成度和进度，如需要，则考虑使用扩展（最好是xAPI实践社区建立的）。

<a name="context"/>

#### <a name="2.4.6">2.4.6</a> Context 内容

###### <a name="2.4.6.s1"></a>Description 描述
一个可选属性，提供了一个可以对语句附加上下文信息的地方，所有的“context”属性都是可选的

###### <a name="2.4.6.s2"></a>Rationale 缘由
可选属性提供了提供了一个可以对语句附加上下文信息的地方，这可以储存例如一个活动的指导者，，如果这个活动是一个基于团队的活动，或者一个活动如何更广泛的融入一个活动。

###### <a name="2.4.6.s3"></a>Details 详情

下表包含了Context object的属性

<table border="1">
<tr><th>Property</th><th>Type</th><th>Description</th><th>Required</th></tr>
<tr id="2.4.6.s3.table1.row1">
	<td>registration</td>
	<td>UUID</td>
	<td>The registration that the Statement is associated with.<br>语句相关的注册</td>
	<td>Optional</td>
</tr>
<tr id="2.4.6.s3.table1.row2">
	<td>instructor</td>
	<td>Agent (MAY be a Group)</td>
	<td>Instructor that the Statement relates to, if not included as the Actor of the Statement.<br>相关语句活动的指导者</td>
	<td>Optional</td>
</tr>
<tr id="2.4.6.s3.table1.row3">
	<td>team</td>
	<td>Group</td>
	<td>Team that this Statement relates to, if not included as the Actor of the Statement.<br>相关语句的团队</td>
	<td>Optional</td>
</tr>
<tr id="2.4.6.s3.table1.row4">
	<td>contextActivities</td>
	<td>contextActivities Object</td>
	<td>A map of the types of learning activity context that this Statement is related to.
	Valid context types are: <code>parent</code>, <code>"grouping"</code>, <code>"category"</code> and <code>"other"</code>.
	<br>一组与语句相关的学习活动内容类型，有效的值是<code>parent</code>, <code>"grouping"</code>, <code>"category"</code> 和 <code>"other"</code>.
	</td>
	<td>Optional</td>
</tr>
<tr id="2.4.6.s3.table1.row5">
	<td>revision</td>
	<td>String</td>
	<td>Revision of the learning activity associated with this Statement. Format is free.<br>相关语句的学习活动的修订，格式无限制</td>
	<td>Optional</td>
</tr>
<tr id="2.4.6.s3.table1.row6">
	<td>platform</td>
	<td>String</td>
	<td>Platform used in the experience of this learning activity.<br>相应学习活动的平台 </td>
	<td>Optional</td>
</tr>
<tr id="2.4.6.s3.table1.row7">
	<td>language</td>
	<td>String (as defined in <a href="http://tools.ietf.org/html/rfc5646">RFC 5646</a>)</td>
	<td>Code representing the language in which the experience being recorded in this 
	Statement (mainly) occurred in, if applicable and known.<br>相应语言的代码
	</td>
	<td>Optional</td>
</tr>
<tr id="2.4.6.s3.table1.row8">
	<td>statement</td>
	<td><a href="#stmtref">Statement Reference</a></td>
	<td>Another Statement to be considered as context for this Statement.<br>另外的一条与该语句相关的语句 </td>
	<td>Optional</td>
</tr>
<tr id="2.4.6.s3.table1.row9">
	<td>extensions</td>
	<td>Object</td>
	<td>A map of any other domain-specific context relevant to this Statement. For example, 
	in a flight simulator altitude, airspeed, wind, attitude, GPS coordinates might all be 
	relevant (<a href="#miscext">See Extensions</a>)<br>扩展。与本语句相关的特定上下文的结构。例如，在一次飞行模拟活动中的高度，风速，姿态，GPS坐标等。参加扩展(<a href="#miscext">See Extensions</a>)</td>
	<td>Optional</td>
</tr>

</table>

###### <a name="2.4.6.s4"></a>Requirements 要求

* <a name="2.4.6.s4.b1"></a>修订“revision”属性MUST 只能在语句的对象（宾语）为活动时使用
* <a name="2.4.6.s4.b2"></a>平台“platform”属性MUST 只能在语句的对象（宾语）为活动时使用
* <a name="2.4.6.s4.b3"></a>语言“language”属性MUST NOT 不能在该语言无法应用的情况下使用
* <a name="2.4.6.s4.b4"></a>修订“revision”属性SHOULD属性应该用于跟踪小问题的修复（如拼写错误）
* <a name="2.4.6.s4.b5"></a>如果活动的学习目标，教育方式或设置发生重大变化，则SHOULD NOT不应使用修订“revision”属性。 （改用新的活动ID）。

__Note:__ 修订“revision”在xAPI的范围内对活动的过程没有实质上的影响。它被简单地存储来以防需要（例如，用于解释和显示数据）.

<a name="Registration"/>

##### <a name="2.4.6.1">2.4.6.1</a> Registration Property 注册属性

###### <a name="2.4.6.1.s1"></a>Rationale/Details 缘由和详情

当LRS是LMS的组成部分时，LMS可能支持注册Registration的概念。xAPI更广泛地应用注册的概念。注册可以被认为是尝试，会话，或可以跨越多个活动。不是说完成活动来结束注册。注册也不一定限于单个代理

当在状态资源中储存文档时，也会使用registration，例如，对于标记书签，通常对于相同活动的语句和状态资源的请求都使用同一个registration，以便于所有的活动记录的数据一致。

<a name="contextActivities"/>

##### <a name="2.4.6.2">2.4.6.2</a> ContextActivities Property 上下文内容属性

###### <a name="2.4.6.2.s1"></a>Description 描述

一系列对于该语句的关于其学习活动上下文的种类

###### <a name="2.4.6.2.s2"></a>Rationale 缘由

许多语句并不仅只聚焦一个活动（对象），而是涉及其他上下文相关结构，“contextActivities”属性用来以结构化的方式表示这些相关活动。

###### <a name="2.4.6.2.s3"></a>Details 详情

有4种上下文类型，每一个或者全都可能使用在语句中:

* <a name="2.4.6.2.s3.b1"></a>__Parent__: 对于语句中的活动（宾语对象），与其有直接关系的活动，多数情况下只会有一个或者没有。例如，对于一个测验问题的语句有着一个测验活动作为其parent
 
* <a name="2.4.6.2.s3.b2"></a>__Grouping__: 对于语句中的活动（宾语对象），与其有非直接关系的活动，例如，一个课程作为一个资质的一部分，而这个课程有7节课，那么这个课程作为这7节课的parent，而这歌资质则作为这7节课的grouping活动

* <a name="2.4.6.2.s3.b3"></a>__Category__: 用于对语句的分类，和标签一个意思，用于标识xAPI的配置类型，例如，Anna,尝试生物学考试，并且使用cmi5 配置，则语句的活动为考试，而类别为cmi5配置

* <a name="2.4.6.2.s3.b4"></a>__Other__: 与上述不同的其他的分类，例如，Anna为了生物考试而学习一本书，语句的活动（宾语）为书，而exam则作为上下文，则contextActivity为other


__Note:__此部分中的值不是用于表示Statement对象具有的所有关系。相反，它们用于表达适合于特定语句的关系（虽然对象的性质在确定时通常很重要）。例如，在关于测试的语句中包括“某课程”作为测试“parent”的部分是适当的，但不包括每个可能的将课程作为一部分的grouping元素。

###### <a name="2.4.6.2.s4"></a>Requirements 要求
* <a name="2.4.6.2.s4.b1"></a>contextActivities上下文活动对象的每一个键MUST必须为parent, grouping, category, 或者 other。
* <a name="2.4.6.2.s4.b2"></a>contextActivities上下文活动对象的每一个值MUST必须为一个活动对象或者一组活动对象
* <a name="2.4.6.2.s4.b3"></a>LRS必须MUST将上下文活动对象的每个值返回为数组array，尽管其接收到时是一个单一的活动对象。
* <a name="2.4.6.2.s4.b4"></a>LRS必须MUST将单个活动对象返回为一个长度为一的数组array。
* <a name="2.4.6.2.s4.b5"></a>学习记录提供者SHOULD应当确保每个上下文活动对象都为一个array而不是一个单一的活动对象。

###### <a name="2.4.6.2.s5"></a>Example 示例

考虑如下梯级形式，问题1-6(Questions 1 to 6)作为测验1(Test 1)的一部分，而测验1又属于课程算法1（Algebra 1）。那么测验1就作为问题1-6的parent，而同时算法1就作为问题1-6的grouping来完成一个最基本的阶梯结构。这在当一个代理作为语句的对象（宾语）时尤其有用，如“安德鲁对于“算法1”的内容指导了本”

```
{
    "parent" : [
        {
            "id" : "http://example.adlnet.gov/xapi/example/test1"
        }
    ],
    "grouping" : [
        {
            "id" : "http://example.adlnet.gov/xapi/example/Algebra1"
        }
    ]
}
```

<a name="timestamp"/>

#### <a name="2.4.7">2.4.7</a> Timestamp 时间戳

###### <a name="2.4.7.s1"></a>Description 描述

活动出现的时间

###### <a name="2.4.7.s2"></a>Details 详情

“timestamp”属性的类型为Timestamp。它根据ISO 8601的正常格式进行格式化，并且对应于在此语句中描述的事件发生的时间。如果在提交到LRS时未包括在语句中，则LRS将使用与存储时使用的值相同的值填充它

Statement中的“timestamp属性”可能与“stored”属性（语句存储的时间）不同。也就是说，在经验的出现和由LRS接收相应的声明之间可能存在延迟。

在经历在一段时间内发生的情况下，“时间戳timestamp”属性可以表示体验期间的开始，结束或任何时间点。将由实践社区将定义一个适当的点来记录不同体验的时间戳。例如，当记录在餐馆吃饭的经历时，记录开始体验的时间戳可能是最合适的;当记录完成资格的经验时，记录经验结束的时间戳可能是最合适的。这些实施例仅用于说明目的，并不意味着是规定性的

###### <a name="2.4.7.s3"></a>Requirements 要求

* <a name="2.4.7.s3.b1"></a>对于Timestamp 数据结构 请参阅 [Section 4.5 ISO 8601 Timestamps](#timestamps).
* <a name="2.4.7.s3.b2"></a>时间戳"timestamp"属性应当SHOULD*被LRS设置为与 ["stored" property](#stored)属性里一样，如果没提供的话 
* <a name="2.4.7.s3.b3"></a>"timestamp"属性可以MAY是活动中的任何一个时间点。
* <a name="2.4.7.s3.b4"></a>一个学习记录提供者不能MUST NOT在当前语句中使用未来的时间点
* <a name="2.4.7.s3.b5"></a>一个子语句可以MAY有一个未来的时间点
* <a name="2.4.7.s3.b6"></a>为了防止是时钟错误，一个LRS  不应当SHOULD* NOT拒绝有着与现在时间相差甚远的时间戳的语句。

<a name="stored"/> 

#### <a name="2.4.8">2.4.8</a> Stored 储存的时间

###### <a name="2.4.8.s1"></a>Description 描述

LRS存储Statement的时间。这可以是LRS收到语句和写入存储之间的任何时间

###### <a name="2.4.8.s2"></a>Details 详情

“stored”属性的类型为 [Timestamp](#timestamps)。就是语句被存储的字面意思的时间.

###### <a name="2.4.8.s3"></a>Requirements 要求

* <a name="2.4.8.s3.b1"></a>对于Timestamp 数据结构 请参阅后文的 [ISO 8601 Timestamps](#timestamps) below.
* <a name="2.4.8.s3.b2"></a>“存储stored”属性必须由LRS设置;一个LRS应该验证，然后必须覆盖当前在它接收的Statement的“stored”属性中的任何值。
* <a name="2.4.8.s3.b3"></a>“存储stored”属性应该是当前或过去的时间。

<a name="authority"/> 

#### <a name="2.4.9">2.4.9</a> Authority 授权

###### <a name="2.4.9.s1"></a>Description 描述

授权authority属性提供了有关谁或者什么声称被语句为真的信息

###### <a name="2.4.9.s2"></a>Details 详情

断言授权表示某些认证的用户，系统或应用程序。

###### <a name="2.4.9.s3"></a>Requirements 要求

* <a name="2.4.9.s3.b1"></a>授权MUST必须是一个代理，除非为第三方认证Oauth，这样的话就必须是具有两个代理的组来分别表示应用和用户。
* <a name="2.4.9.s3.b2"></a>如果用户直接连接（使用HTTP基本身份验证）或作为组的一部分包括在内，LRS必须将用户作为代理视为整个权限 
* <a name="2.4.9.s3.b3"></a>LRS 必须MUST保证所有的语句都有授权
* <a name="2.4.9.s3.b4"></a>LRS应该根据用于发送这些语句的凭证，覆盖其存储的所有语句的权限
* <a name="2.4.9.s3.b5"></a>LRS可能使提交的权限保持不变，但只有在建立强烈的信任关系并且非常谨慎的情况下才这样做。
* <a name="2.4.9.s3.b6"></a>如果用户直接连接（使用HTTP基本身份验证）或使用三方模式OAuth的一部分，则LRS可以为用户标识任何合法的标识属性。

##### <a name="2.4.9.s4"></a>OAuth Credentials as Authority 以OAuth 证书 作为认证

###### <a name="2.4.9.s5"></a>Description 描述

使用OAuth的工作流程，支持2-legged和3-legged OAuth。

###### <a name="2.4.9.s6"></a>Details

此工作流假定使用已验证的OAuth连接存储Statement，并且LRS创建或修改Statement的权限属性

在三方OAuth工作流程中，身份验证涉及OAuth使用者和OAuth服务提供商的用户。例如，由经授权的Twitter插件在其Facebook帐户上发出的请求将包含不只是Twitter作为客户端或者作为user而已，而是二者的结合。

###### <a name="2.4.9.s7"></a>Requirements 要求
 
* <a name="2.4.9.s7.b1"></a>授权authority必须包含作为代表OAuth使用者的Agent Object，不论是其自己还是在三方OAuth情况下作为group的一部分。
* <a name="2.4.9.s7.b2"></a>代表OAuth客户的代理MUST必须通过账户标识。
* <a name="2.4.9.s7.b3"></a>代表OAuth客户的代理必须MUST使用consumer键作为帐户的“name”属性的值
* <a name="2.4.9.s7.b4"></a>如果代表OAuth使用者的代理是注册的应用程序，则令牌请求端点必须用作帐户的“homePage”属性的值。
* <a name="2.4.9.s7.b5"></a>如果代表OAuth使用者的代理程序不是注册的应用程序，则临时凭证端点必须用作帐户的“homePage”属性的值。
* <a name="2.4.9.s7.b6"></a>在帐户名与未注册的应用程序来自相同的源的情况下，LRS不得信任权限的应用程序部分。 （多个未注册的应用程序可以选择相同的使用者密钥。因此，没有一致的方法来验证此临时凭证和帐户名的组合。）
* <a name="2.4.9.s7.b7"></a>每个未注册的客户应该SHOULD使用唯一的客户密钥。

###### <a name="2.4.9.s8"></a>Example 示例

The pairing of an OAuth consumer and a user.

```
"authority": {
	"objectType" : "Group",
	"member": [
		{
			"account": {
				"homePage":"http://example.com/xAPI/OAuth/Token",
				"name":"oauth_consumer_x75db"
			}
		},
		{ 
			"mbox":"mailto:bob@example.com" 
		}
	]
}
```

<a name="version"/> 

#### <a name="2.4.10">2.4.10</a> Version 版本
###### <a name="2.4.10.s1"></a>Description 描述

Statement中的版本信息有助于学习记录消费者获得自己的方向。由于Statement数据模型通过所有1.0.x版本保证一致，为了支持这些LRS之间的数据流，LRS在接受的Statement版本上有一定的灵活性。

###### <a name="2.4.10.s2"></a>Requirements 要求

* <a name="2.4.10.s2.b1"></a>版本必须格式化为[Versioning](./xAPI-Communication.md#versioning)中的API版本头

###### <a name="2.4.10.s3"></a>LRS Requirements 对LRS的要求

* <a name="2.4.10.s3.b1"></a>LRS必须MUST接受所有以`1.0.`开头版本的语句
* <a name="2.4.10.s3.b2"></a>LRS必须MUST拒绝所有具有指定版本且不以`1.0.`开头的语句 .
* <a name="2.4.10.s3.b3"></a>LRS返回的语句必须保留它们接受的版本。如果他们没有版本，版本必须设置为 `1.0.0`.


###### <a name="2.4.10.s4"></a>Learning Record Provider Requirements 对LRP的要求

* <a name="2.4.10.s4.b1"></a>如果学习记录提供者设置语句版本，它们必须将其设置为 `1.0.0`.
* <a name="2.4.10.s4.b2"></a>学习记录提供者不应该设置Statement版本

__Note:__ 对于“version”属性包含值`1.0.0`而不是最新修补程序版本的要求是慎重的，因为任何版本的1.0.x中的语句都符合1.0.0数据模型。事实上，随着时间的推移，单个语句可能会包含在多个请求中，每个都在规范的不同补丁版本之后。可以从在每个请求中使用的["X-Experience-API-Version" header](./xAPI-Communication.md#versioning)报头确定遵循的规范的补丁版本。

<a name="attachments"/>
#### <a name="2.4.11">2.4.11</a> Attachments 附件

###### <a name="2.4.11.s1"></a>Rationale 缘由

在某些情况下，附件在逻辑上是学习记录的重要组成部分。它可以是文章，视频等。这种附件的另一个示例是作为经历的结果而被授予的证书（的图像）。有一种方法来存储这些附件并从LRS中检索它们是非常有用的

###### <a name="2.4.11.s2"></a>Details 详情

下表列出了附件对象Attachment Object的所有属性

<table>
	<tr><th>Property</th><th>Type</th><th>Description</th><th>Required</th><th>Corresponding request parameter</th></tr>
	<tr id="2.4.11.s2.table1.row1">
		<a name="attachmentUsage" />

		<td>usageType</td>
		<td>IRI</td>
		<td>Identifies the usage of this Attachment. For example: one expected use case
		for Attachments is to include a "completion certificate". An IRI corresponding
		to this usage MUST be coined, and used with completion certificate attachments. <br>标识此附件的用法。例如：附件的一个预期用例是包括“完成证书”。与此用法相对应的IRI必须被创造，并与完成证书附件一起使用。</td>
		<td>Required</td>
		<td></td>
	</tr>
	<tr id="2.4.11.s2.table1.row2">
		<td>display</td>
		<td><a href="#lang-maps">Language Map</a></td>
		<td>Display name (title) of this Attachment.<br>此附件的显示名称（标题）。</td>
		<td>Required</td>
		<td></td>
	</tr>
	<tr id="2.4.11.s2.table1.row3">
		<td>description</td>
		<td><a href="#lang-maps">Language Map</a></td>
		<td>A description of the Attachment<br>附件说明</td>
		<td>Optional</td>
		<td></td>
	</tr>
	<tr id="2.4.11.s2.table1.row4">
		<td>contentType</td>
		<td><a href="https://www.ietf.org/rfc/rfc2046.txt?number=2046">Internet Media Type</a></td>
		<td>The content type of the Attachment.<br>附件内容类型</td>
		<td>Required</td>
		<td>Content-Type</td>
	</tr>
	<tr id="2.4.11.s2.table1.row5">
		<td>length</td>
		<td>Integer</td>
		<td>The length of the Attachment data in octets.<br>附件数据的长度（以字节为单位）</td>
		<td>Required</td>
		<td>Content-Length</td>
	</tr>
	<tr id="2.4.11.s2.table1.row6">
		<td>sha2</td>
		<td>String</td>
		<td>The SHA-2 hash of the Attachment data. <br/>
		This property is always required, even if fileURL is also specified. <br>附件数据的SHA-2散列。此属性始终是必需的，即使还指定了fileURL。
		</td>
		<td>Required</td>
		<td>X-Experience-API-Hash</td>
	</tr>
	<tr id="2.4.11.s2.table1.row7">
		<td>fileUrl</td>
		<td>IRL</td>
		<td>An IRL at which the Attachment data can be retrieved, or from which it used 
		to be retrievable. <br>可以检索附件数据或是从中可以检索到附件数据的IRL。</td>
        <td>Optional</td>
		<td></td>
	</tr>
</table>

在希望包含子语句的附件的情况下，强烈建议在Statement的Attachment对象中包含附件，并包括通常对语句所做的有效内容。

<a name="retrieval"/> 
### <a name="2.5">2.5</a> Retrieval of Statements 语句的检索

###### <a name="2.5.s1"></a>Description 描述

可以通过对语句资源执行查询来检索语句集合，有关详细信息，请参阅 [Statement Resource](./xAPI-Communication.md#stmtres)语句资源。 

###### <a name="2.5.s2"></a>Details 详情

下表显示了对语句资源的查询结果的数据结构。
<table>
	<tr><th>Property</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="2.5.s2.table1.row1"><td>statements</td><td>Array of Statements</td>
		<td>List of Statements. If the list returned has been limited (due to pagination), 
			and there are more results, they will be located at the "statements" property 
			within the container located at the IRL provided by the "more" property of 
			this Statement result Object.
			
			Where no matching Statements are found, this property will contain an empty array. <br>语句列表。如果返回的列表已被限制（由于分页），并且有更多结果，它们将位于由此Statement对象的“more”属性提供的IRL中的容器中的“statements”属性。如果没有找到匹配的语句，此属性将包含一个空数组。
		</td>
		<td>Required</td>
	</tr>
	<tr id="2.5.s2.table1.row2"><td>more</td><td>IRL</td>
		<td>Relative IRL that can be used to fetch more results, including the full path 
			and optionally a query string but excluding scheme, host, and port. 
			Empty string if there are no more results to fetch.<br>可用于获取更多结果的相对IRL，包括完整路径和可选的查询字符串，但不包括方案，主机和端口。如果没有更多结果要提取，则为空字符串
		</td>
		<td>Required if the list returned has been limited, otherwise optional.<br>如果返回的列表已被限制，则为必需，否则为可选</td>
	</tr>
</table>

###### <a name="2.5.s3"></a>Requirements 要求

* <a name="2.5.s3.b1"></a>从“more”属性检索到的IRL必须MUST在LRS返回后至少24小时内可用
* <a name="2.5.s3.b2"></a>LRS可以MAY在 “more”属性IRL中包括所有必要信息，以继续查询，从而避免存储IRL和关联查询数据。
* <a name="2.5.s3.b3"></a>LRS不应该SHOULD NOT在“more”属性中生成超长的IRL。
* <a name="2.5.s3.b4"></a>LRS可以在访问从“more”属性检索到的IRL时立即重新查询，如果在LRS中存在的话，会使得所检索的批拥有将被包括在该批中的语句，并排除该批次中已被无效的语句。
* <a name="2.5.s3.b5"></a>或者，LRS可以缓存要在“more”属性返回的语句的列表，使得返回的语句批次与在运行原始查询时将返回的语句相匹配
* <a name="2.5.s3.b6"></a>如果使用此方法，LRS可以从缓存的语句列表中删除voided语句。
* <a name="2.5.s3.b7"></a>学习记录消费者不应试图解释从“more”属性返回的IRL的任何含义。

<a name="signature"/>
### <a name="2.6">2.6</a> Signed Statements 签名语句

##### <a name="2.6.s1"></a>Description 描述

语句可以包括数字签名[digital signature](https://en.wikipedia.org/wiki/Digital_signature)，以提供有力和持久的声明的真实性和完整性的证据。 


##### <a name="2.6.s2"></a>Rationale 缘由

一些语句将具有监管或法律意义，或以其他方式要求其真实性和完整性的强有力和持久的证据。可能有必要验证这些语句，而不信任他们首次记录的环境，或者可能无法访问该环境。数字签名将使第三方能够验证此类语句。

##### <a name="2.6.s3"></a>Details 详情

签名语句包括作为附件的JSON Web签名（JWS）。这允许语句的原始系列化将签名一起包括了起来。为了实现交互性，选择了“RSA + SHA”系列JWS算法，并且为了签名者的可见性，应使用X.509证书。

##### <a name="2.6.s4"></a>Signature Requirements 对签名的要求
* <a name="2.6.s4.b1"></a>签名语句必须包含如下定义的Web签名（JWS）：
http://tools.ietf.org/html/rfc7515 ,在附件中以 `http://adlnet.gov/expapi/attachments/signature`来作为usageType 和 `application/octet-stream`来作为contentType
* <a name="2.6.s4.b2"></a>JWS紧凑序列化应该用于创建JSON Web签名。使用JWS JSON序列化是强烈不推荐的，这会导致不可能与其他系统互操作，并且将在本规范的未来版本中被禁止。
* <a name="2.6.s4.b3"></a>在添加签名之前，JWS签名必须具有有效的JSON序列化的有效载荷。
* <a name="2.6.s4.b4"></a>JWS签名必须使用“RS256”，“RS384”或“RS512”算法。
* <a name="2.6.s4.b5"></a>JWS签名应该基于与X.509证书相关联的私钥创建。
* <a name="2.6.s4.b6"></a>如果使用X.509进行签名，JWS头应该包含包含相关证书链的“x5c”属性。

##### <a name="2.6.s5"></a>LRS Requirements 对LRS的要求
* <a name="2.6.s5.b1"></a>LRS必须拒绝存储包含格式不正确的签名的语句的请求，具有400错误请求。`400 Bad Request`.
* <a name="2.6.s5.b2"></a>LRS应该在被拒绝的语句的响应中包括一条消息。
* <a name="2.6.s5.b3"></a>为了使得验证的签名具有好的格式，LRS必须遵守
    * <a name="2.6.s5.b3.b1"></a>解码JWS签名，并从JWS签名有效载荷加载Statement的签名序列化。
    * <a name="2.6.s5.b3.b2"></a>验证原始语句在逻辑上等同于接收的语句。见[Statement comparision requirements](#statement-comparison-requirements).
    * <a name="2.6.s5.b3.b3"></a>如果JWS头包含X.509证书，则根据JWS中定义的该证书验证签名。
    * <a name="2.6.s5.b3.b4"></a>验证是否满足上述签名要求

__Note:__ 针对包括的X.509证书进行验证的步骤旨在作为捕获签名中的错误的方式，而不是作为安全措施。验证签名的语句的步骤将根据所需的确定性程度而变化，并且超出本规范的范围。

##### <a name="2.6.s6"></a>Client Requirements 对客户的要求

* <a name="2.6.s6.b1"></a>客户必须遵守上述签名要求。
* <a name="2.6.s6.b2"></a>客户不得只是因为LRS已经接受它，就假设签名有效。



##### <a name="2.6.s7"></a>Example 示例

例子参见 [Appendix D: Example Signed Statement](#Appendix2D)

<a name="metadata"/>

## <a name="3.0">3.0</a> Metadata 元数据

元数据是关于资源的附加信息。它被利用在决策，搜索和可发现性。在xAPI中，元数据可以在各种位置中使用。最常见的是在活动定义中。

<a name="iri-requirements"/>

### <a name="3.1">3.1</a> IRI Requirements IRI要求

xAPI使用IRI作为标识符。使用IRI可确保唯一性并提高可解析性。如下所述，LRS和学习记录提供者都分别对每个IRI的职责。在活动定义中有其他规则，可以在这里找到。 [here](#actdef)

##### <a name="3.1.s1"></a>Metadata Provider Requirements 对元数据提供者的要求

这些要求也适用于定义新IRI的学习记录提供者。

* <a name="3.1.s1.b1"></a>[Metadata Providers 元数据提供者](./xAPI-About.md#def-metadata-provider) 在定义新的IRI时，应该SHOULD*使用在他们控制范围内的IRI。
* <a name="3.1.s1.b2">元数据提供者在定义新的Verb IRI时，必须MUST使用在他们控制范围内的IRI。
* <a name="3.1.s1.b3"></a>在合适的标识符已经存在的情况下，元数据提供者应该使用相应的现有标识符，并且不应该创建新的标识符。
* <a name="3.1.s1.b4"></a>当重新使用现有标识符时，元数据提供者应该确保使用确切的字符等价的IRI
* <a name="3.1.s1.b5"></a>元数据提供者可以创建自己的标识符，如果其中合适的标识符不存在的话。
* <a name="3.1.s1.b6"></a>定义标识符时，元数据提供者可以使用包含定位点的IRI，以便单个页面可以包含多个标识符的定义。例如： `http://example.com/xapi/verbs#defenestrated`
* <a name="3.1.s1.b7"></a>定义标识符时，元数据提供者应该使用小写的IRI。

##### <a name="3.1.s2"></a>LRS Requirements LRS哟求

* <a name="3.1.s2.b1"></a>当存储或比较IRI时，LRS应该仅使用RFC 3987的5.3.1（简单字符串比较）[5.3.1 (Simple String Comparison)和5.3.2（基于语法的规范化）5.3.2 (Syntax-Based Normalization) of RFC 3987](https://tools.ietf.org/html/rfc3987#section-5.3)中描述的一种或多种方法来处理它们，并且应当SHOULD *使用相同RFC的5.3.3（基于方案的规范化）或5.3.4（基于协议的规范化）[5.3.3 (Scheme-Based Normalization) or 5.3.4 (Protocol-Based Normalization) of the same RFC](https://tools.ietf.org/html/rfc3987#section-5.3)或任何其他方法中描述的任一方法。  
* <a name="3.1.s2.b2"></a>LRSs 应当SHOULD *应用相同的IRI比较和规范化规则对于包含IRI的参数和字段的所有IRI。
<a name="miscmeta"/>

### <a name="3.2">3.2</a> Hosted Metadata 站点元数据

##### <a name="3.2.s1"></a>Description 描述

关于标识的额外的信息可以被放在被IRI所指定的站点上，包含在语句中的元数据使得关于IRI的元数据能够不需要解析的情况下使用它，而储存在站点上的元数据使得IRI的持有者能够定义其规范。

##### <a name="3.2.s2"></a>Details 详情

在本规范中，有以下几类IRI标识：

* <a name="3.2.s2.b1"></a>[Verb](#verb)
* <a name="3.2.s2.b2"></a>[Activity id](#acturi)
* <a name="3.2.s2.b3"></a>[Activity type](#acttype)
* <a name="3.2.s2.b4"></a>[extension key](#miscext)
* <a name="3.2.s2.b5"></a>[attachment usage type](#attachmentUsage)

有关活动ID的站点元数据的结构，请参阅活动定义对象。 [Activity Definition Object](#activity).

有关所有的站点元数据的结构，参见下格式

<table>
	<tr><th>Property</th><th>Type</th><th>Description</th><th>Required</th></tr>
	<tr id="3.2.s2.table1.row1">
		<td>name</td>
		<td><a href="#lang-maps">Language Map</a></td>
		<td>The human readable/visual name. For Verbs, this is equivalent to the "display" property in a Statement.<br>人类可读/视觉名称。对于动词，这相当于Statement中的“display”属性。</td>
		<td>Optional</td>
	</tr>
	<tr id="3.2.s2.table1.row2">
		<td>description</td>
		<td><a href="#lang-maps">Language Map</a></td>
		<td>description<br>描述</td>
		<td>Optional</td>
	</tr>
</table>

站点元数据由包含上述JSON对象的文档组成，如果提供此站点元数据，则它是关于其描述的标识符的规范信息源，除了Activity id之外的所有类型的IRI标识符，建议实现xAPI的人查找和使用已经建立的被广泛采用的标识符。

##### <a name="3.2.s3"></a>Metadata Provider Requirements 对元数据提供者的要求

* <a name="3.2.s3.b1"></a>元数据可以MAY随着一个标识来提供
* <a name="3.2.s3.b2"></a>如果提供了元数据，那么相应的“名称name”和“描述description”都该提供
* <a name="3.2.s3.b3"></a>对于元数据提供者上面的任何标识符IRI，应该对IRI上可访问的预期用途进行人类可读的描述。
* <a name="3.2.s3.b4"></a>对于元数据提供者上面的任何标识符IRI，应当在请求IRI时用 内容类型`application/json`时，确保该IRI处的该JSON元数据可用。
* <a name="3.2.s3.b5"></a>在IRI表示活动的情况下，元数据提供者可以使用在语句中使用的[活动定义Activity Definition](#actdef)JSON格式来存放元数据，其具有内容类型 `application/json` 

##### <a name="3.2.s4"></a>LRS Requirements 对LRS的要求

* <a name="3.2.s4.b1"></a>LRS可能充当[元数据使用者Metadata Consumer](./xAPI-About.md#def-metadata-consumer)并尝试解析标识符IRI。  
* <a name="3.2.s4.b2"></a>如果活动IRI是一个URL，LRS应该尝试获取该URL，并包括在HTTP头中： `Accept: application/json, */*`。这应该在LRS首次遇到活动ID后尽快实施。
* <a name="3.2.s4.b3"></a>在从用作活动ID的URL中加载作为有效活动定义的JSON时，LRS应该将加载的定义合并到该活动的规范定义中，同时保留未包含在加载的定义中的名称或定义。
* <a name="3.2.s4.b4"></a>加载任何文档，LRS可以从用作活动ID的URL解析活动定义时，LRS可以在确定其活动定义的规范表示时考虑此定义
its canonical representation of that Activity's definition.

##### <a name="3.2.s5"></a>Metadata Consumer Requirements 对元数据消费者的要求

* <a name="3.2.s5.b1"></a>如果元数据消费者从IRI获得元数据，它应该强烈推测在该IRI中找到的元数据对于该元数据中包括的属性和语言是权威的。
* <a name="3.2.s5.b2"></a>元数据消费者可以使用其他信息来填充缺少的详细信息（例如翻译），或者完全代替托管的元数据（如果未提供），无法加载或元数据使用者不信任它。其他信息源可以包括存储在标识符的IRI处的其他格式的元数据，特别是如果该标识符不是为了与本说明书一起使用而创建的。


<a name="special-data"/>

## <a name="4.0">4.0</a> Special Data Types and Rules 特殊的数据类型和规则

以下是在本说明书中常见的需要附加规则的数据类型。

<a name="miscext"/> 

### <a name="4.1">4.1</a> Extensions 扩展

##### <a name="4.1.s1"></a>Description 描述

扩展可作为活动定义的一部分，作为语句的“上下文”属性的一部分，或作为语句的“result”属性的一部分。在每种情况下，扩展旨在提供一种自然的方式来扩展那些属性以用于某些专门用途。这些扩展的内容可能只对一个应用程序有价值，或者它可能是一个完整的实践社区使用的约定

##### <a name="4.1.s2"></a>Details 详情

扩展由映射定义，并在逻辑上与它们所在的语句的部分相关。扩展的值可以是任何JSON值或数据结构。 “context”属性中的扩展为核心体验提供上下文，而“result”属性中的扩展提供与某些结果相关的元素。在活动内，扩展提供了其他信息，有助于在某些自定义应用程序或实践社区中定义活动。 IRI密钥下的扩展值的含义和结构由控制IRI的人员定义。

##### <a name="4.1.s3"></a>Requirements 要求

* <a name="4.1.s3.b1"></a>扩展映射的键必须是IRI
* <a name="4.1.s3.b2"></a>LRS不得基于扩展映射的值拒绝语句。
* <a name="4.1.s3.b3"></a>学习记录提供者应该总是努力将尽可能多的信息映射到内置元素中，以便利用x API一致性工具之间的互操作性。
* <a name="4.1.s3.b4"></a>所有扩展IRI应该有持有者
* <a name="4.1.s3.b5"></a>IRL扩展密钥的持有者应该对IRL可访问的IRL支持的扩展的预期含义进行人类可读的描述。

__Note:__ 完全由其扩展定义的语句变得没有意义，因为没有其他系统能够理解它。

<a name="lang-maps"/> 

### <a name="4.2">4.2</a> Language Maps 语言映射

##### <a name="4.2.s1"></a>Description 描述

Language map是键为 [RFC 5646 Language Tag](http://tools.ietf.org/html/rfc5646)语言标记字典中的词，且值为标记中指定的语言字符串的表达映射。这个映射应该根据不同语言中的知识尽可能完整的填充。

通常优选每个语言字符串中最短的代码，[ISO 639 language code 语言代码](https://www.loc.gov/standards/iso639-2/php/code_list.php)加上[ISO 3166-1 country code 国家代码](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)允许指定基本语言（例如`es`用于西班牙语）和区域（例如，`es-MX`，西班牙语在墨西哥语的方言）。如果只有ISO 639语言代码是已知的，不要猜测可能的ISO 3166-1国家代码。例如，如果只知道主要语言（例如，英语），则使用顶级语言标记`en`，而不是`en-US`。如果已知特定区域变体，请使用完整的语言代码。


__Note:__ 对于中文，由zh表示的重要语言多样性意味着ISO 639语言代码通常不足

语言映射中的字符串的内容是纯文本。预期任何格式化代码（例如HTML标记或markdown）都不会被呈现，但是当此字符串显示给最终用户时将显示为代码。一个重要的例外是如果在扩展中使用语言映射Object，并且该扩展的所有者IRI明确地声明将呈现特定形式的代码。

<a name="iris"/>

### <a name="4.3">4.3</a> IRIs 

国际化资源标识符或IRI是也是可解析的唯一标识符。因为不需要解析，所以使用IRI / URI而不是IRL / URL。为了允许在标识符中使用的字符的最大灵活性，使用IRI而不是URI，因为IRI可以包含ASCII字符集之外的一些字符。

参见[Metadata 元数据](#metadata). 

<a name="uuids"/>

### <a name="4.4">4.4</a> UUIDs

通用唯一标识符或UUID是全局唯一的128位值。与IRI不同，由于UUID采用完全不同的格式，因此没有预期的可解析性。 UUID必须是标准字符串形式。建议使用[RFC 4122](http://tools.ietf.org/html/rfc4122)中的变体2。

<a name="timestamps"/>

### <a name="4.5">4.5</a> ISO 8601 Timestamps 时间戳

时间戳是表示特定时间的格式类型。它们根据ISO 8601的正常格式进行格式化。发送到LRS的语句可以保持精度至少为毫秒

###### <a name="4.5.s1"></a>Requirements 要求
* <a name="4.5.s1.b1"></a>时间戳必须根据[ISO 8601](https://en.wikipedia.org/wiki/ISO_8601#Combined_date_and_time_representations)格式化.
* <a name="4.5.s1.b2"></a>时间戳应该使用RFC 3339中描述的格式表示， [RFC 3339](https://www.ietf.org/rfc/rfc3339.txt)是ISO 8601的配置文件
* <a name="4.5.s1.b3"></a>时间戳必须保持精度至少毫秒（超过秒的3个小数点）
* <a name="4.5.s1.b4"></a>时间戳应该包含时区•
* <a name="4.5.s1.b5"></a>如果时间戳包括时区，则LRS可以使用不同的时区将时间戳返回到语句中最初使用的时区，只要所参考的时间点不受影响
* <a name="4.5.s1.b6"></a>LRS 应当SHOULD *返回UTC时区中的时间戳。
* <a name="4.5.s1.b7"></a>时间戳可以被截断或舍入到精度至少为三位十进制数字的秒。
<a name="durations"/>

### <a name="4.6">4.6</a> ISO 8601 Durations 持续时间

持续时间是表示某事花费的时间量的字符串

###### <a name="4.6.s1"></a>Requirements 要求

* <a name="4.6.s1.b1"></a>持续时间必须使用ISO 8601：2004（E）第4.4.3.2节中的持续时间格式表示。不得使用替代格式（与用于时间点的格式一致，并在ISO 8601：2004（E）第4.4.3.3节中描述）。
* <a name="4.6.s1.b2"></a>学习记录提供者应该提供0.01秒的最大精度
* <a name="4.6.s1.b3"></a>学习记录提供者可能提供较低的精度，例如在获得大学学位的情况下精度可能是几个月或几年。
* <a name="4.6.s1.b4"></a>在接收到超过0.01秒精度的持续时间时，LRS应该不拒绝请求，但可以将“持续时间”属性截断为0.01秒精度。
* <a name="4.6.s1.b5"></a>当比较持续时间时，超过0.01秒精度的任何精度应该不包括在比较中。

###### <a name="4.6.s2"></a>Examples 示例

下表提供了一些ISO 8601持续时间的示例。此列表并不旨在详尽无遗

<table>
	<tr><th>Example</th><th>Explanation</th></tr>
	<tr id="4.6.s2.table1.row1">
		<td>PT4H35M59.14S</td>
		<td>Four hours, thirty five minutes and 59.14 seconds.<br>四小时，三十五分钟和59.14秒</td>
	</tr>
	<tr id="4.6.s2.table1.row2">
		<td>P16559.14S</td>
		<td>The same time period as above represented in seconds. 
		(Note: if the time period in question contained a leap second, this conversion would be inaccurate)<br>与上述相同的时间段以秒为单位。 （注意：如果所涉及的时间段包含闰秒，则此转换将不准确）</td>
	</tr>
	<tr id="4.6.s2.table1.row3">
		<td>P3Y1M29DT4H35M59.14S</td>
		<td>A Duration also including years, months and days.<br>包括年月日的持续时间</td>
	</tr>
	<tr id="4.6.s2.table1.row4">
		<td>P3Y</td>
		<td>Approximately three years e.g. completion of a qualification.<br>大约三年完成资格</td>
	</tr>
	<tr id="4.6.s2.table1.row5">
		<td>P4W</td>
		<td>Four weeks. Note that weeks cannot be combined with other time periods. 'P4W1D' is not valid.<br>4周,请注意，星期不能与其他时间段组合。 例，'P4W1D'是无效的。</td>
	</tr>
</table>

推荐以记录它们的格式来呈现期间。例如，如果以秒（或几分之一秒）跟踪持续时间，则不需要将其转换为小时，分钟和秒。

<a name="append2"/>
## <a name="4.6.s3"></a>Appendices 附录
<a name="Appendix2A"/>  
 
### <a name="A">Appendix A</a>: Example Statements 示例语句

Example of a simple Statement (line breaks are for display purposes only):  
```
{
	"id":"fd41c918-b88b-4b20-a0a5-a4c32391aaa0",
	"timestamp": "2015-11-18T12:17:00+00:00",
	"actor":{
		"objectType": "Agent",
		"name":"Project Tin Can API",
		"mbox":"mailto:user@example.com"
	},
	"verb":{
		"id":"http://example.com/xapi/verbs#sent-a-statement",
		"display":{ 
			"en-US":"sent" 
		}
	},
	"object":{
		"id":"http://example.com/xapi/activity/simplestatement",
		"definition":{
			"name":{ 
				"en-US":"simple statement" 
			},
			"description":{ 
				"en-US":"A simple Experience API statement. Note that the LRS 
				does not need to have any prior information about the Actor (learner), the 
				verb, or the Activity/object." 
			}
		}
	}
}
```   
Completion with Verb named "attempted" and Duration expressed in seconds (not converted to minutes and seconds):  
加入了动词“参加”，并且持续时间用秒（没有转换为几分几秒）来表示的例子。
```
{
	"id":"7ccd3322-e1a5-411a-a67d-6a735c76f119",
	"timestamp": "2015-12-18T12:17:00+00:00",
	"actor":{
        "objectType": "Agent",
		"name":"Example Learner",
		"mbox":"mailto:example.learner@adlnet.gov"
	},
	"verb":{
		"id":"http://adlnet.gov/expapi/verbs/attempted",
		"display":{
			"en-US":"attempted"
		}
	},
	"object":{
		"id":"http://example.adlnet.gov/xapi/example/simpleCBT",
		"definition":{
			"name":{
				"en-US":"simple CBT course"
			},
			"description":{
				"en-US":"A fictitious example CBT course."
			}
		}
	},
	"result":{
		"score":{
			"scaled":0.95
		},
		"success":true,
		"completion":true,
		"duration": "PT1234S"
	}
}
```  
A long example Statement showcasing most of the properties available. This example shows
a Statement returned by an LRS including the "authority" and "stored" properties set by the LRS:  
一个较为长的例子，几乎展示了所有可能的属性，例子展示了一个由LRS设置并返回的包含了“授权”和“储存”。
```
{
    "id": "6690e6c9-3ef0-4ed3-8b37-7f3964730bee",
    "actor": {
        "name": "Team PB",
        "mbox": "mailto:teampb@example.com",
        "member": [
            {
                "name": "Andrew Downes",
                "account": {
                    "homePage": "http://www.example.com",
                    "name": "13936749"
                },
                "objectType": "Agent"
            },
            {
                "name": "Toby Nichols",
                "openid": "http://toby.openid.example.org/",
                "objectType": "Agent"
            },
            {
                "name": "Ena Hills",
                "mbox_sha1sum": "ebd31e95054c018b10727ccffd2ef2ec3a016ee9",
                "objectType": "Agent"
            }
        ],
        "objectType": "Group"
    },
    "verb": {
        "id": "http://adlnet.gov/expapi/verbs/attended",
        "display": {
            "en-GB": "attended",
            "en-US": "attended"
        }
    },
    "result": {
        "extensions": {
            "http://example.com/profiles/meetings/resultextensions/minuteslocation": "X:\\meetings\\minutes\\examplemeeting.one"
        },
        "success": true,
        "completion": true,
        "response": "We agreed on some example actions.",
        "duration": "PT1H0M0S"
    },
    "context": {
        "registration": "ec531277-b57b-4c15-8d91-d292c5b2b8f7",
        "contextActivities": {
            "parent": [
                {
                    "id": "http://www.example.com/meetings/series/267",
                    "objectType": "Activity"
                }
            ],
            "category": [
                {
                    "id": "http://www.example.com/meetings/categories/teammeeting",
                    "objectType": "Activity",
                    "definition": {
			            "name": {
			                "en": "team meeting"
			            },
			            "description": {
			                "en": "A category of meeting used for regular team meetings."
			            },
			            "type": "http://example.com/expapi/activities/meetingcategory"
			        }
                }
            ],
            "other": [
                {
                    "id": "http://www.example.com/meetings/occurances/34257",
                    "objectType": "Activity"
                },
                {
                    "id": "http://www.example.com/meetings/occurances/3425567",
                    "objectType": "Activity"
                }
            ]
        },
        "instructor" :
        {
        	"name": "Andrew Downes",
            "account": {
                "homePage": "http://www.example.com",
                "name": "13936749"
            },
            "objectType": "Agent"
        },
        "team":
        {
        	"name": "Team PB",
        	"mbox": "mailto:teampb@example.com",
        	"objectType": "Group"
        }, 
        "platform" : "Example virtual meeting software",
        "language" : "tlh",
        "statement" : {
        	"objectType":"StatementRef",
        	"id" :"6690e6c9-3ef0-4ed3-8b37-7f3964730bee"
        }
        
    },
    "timestamp": "2013-05-18T05:32:34.804+00:00",
    "stored": "2013-05-18T05:32:34.804+00:00",
    "authority": {
        "account": {
            "homePage": "http://cloud.scorm.com/",
            "name": "anonymous"
        },
        "objectType": "Agent"
    },
    "version": "1.0.0",
    "object": {
        "id": "http://www.example.com/meetings/occurances/34534",
        "definition": {
            "extensions": {
                "http://example.com/profiles/meetings/activitydefinitionextensions/room": {"name": "Kilby", "id" : "http://example.com/rooms/342"}
            },
            "name": {
                "en-GB": "example meeting",
                "en-US": "example meeting"
            },
            "description": {
                "en-GB": "An example meeting that happened on a specific occasion with certain people present.",
                "en-US": "An example meeting that happened on a specific occasion with certain people present."
            },
            "type": "http://adlnet.gov/expapi/activities/meeting",
            "moreInfo": "http://virtualmeeting.example.com/345256"
        },
        "objectType": "Activity"
    }
}
```  
<a name="Appendix2B"/>  

### <a name="B">Appendix B</a>: Examples of Statement's Objects of different types

The Object of a Statement can be an Activity, an Agent, a Group or a Statement. 
This appendix provides one example of each. 

###### <a name="B.s1"></a>Object is Activity
```
{
    "id": "http://www.example.co.uk/exampleactivity",
    "definition": {
        "name": {
            "en-GB": "example activity",
            "en-US": "example activity"
        },
        "description": {
            "en-GB": "An example of an activity",
            "en-US": "An example of an activity"
        },
        "type": "http://www.example.co.uk/types/exampleactivitytype"
    },
    "objectType": "Activity"
}
```

###### <a name="B.s2"></a>Object is Agent
```
{
    "name": "Andrew Downes",
    "mbox": "mailto:andrew@example.co.uk",
    "objectType": "Agent"
}
```

###### <a name="B.s3"></a>Object is Group

This example shows an Identified Group with members. 
```
{
    "name": "Example Group",
    "account" : {
    	"homePage" : "http://example.com/homePage",
    	"name" : "GroupAccount"
    },
    "objectType": "Group",
    "member": [
        {
            "name": "Andrew Downes",
            "mbox": "mailto:andrew@example.com",
            "objectType": "Agent"
        },
        {
            "name": "Aaron Silvers",
            "openid": "http://aaron.openid.example.org",
            "objectType": "Agent"
        }
    ]
}
```


###### <a name="B.s4"></a>Object is Statement

This example shows a SubStatement Object whose Object is a Statement Reference.

```
{
    "objectType": "SubStatement",
    "actor" : {
        "objectType": "Agent", 
        "mbox":"mailto:agent@example.com" 
    },
    "verb" : { 
        "id":"http://example.com/confirmed", 
        "display":{
            "en":"confirmed"
        } 
    },
    "object": {
        "objectType":"StatementRef",
		"id" :"9e13cefd-53d3-4eac-b5ed-2cf6693903bb"
    }
}
```

<a name="Appendix2C"/>  

### <a name="C">Appendix C</a>: Example definitions for Activities of type `cmi.interaction`

###### <a name="C.s1"></a>true-false

```
"definition": {
	"description": {
		"en-US": "Does the xAPI include the concept of statements?"
	},
	"type": "http://adlnet.gov/expapi/activities/cmi.interaction",
	"interactionType": "true-false",
	"correctResponsesPattern": [
		"true"
	]
}
```

###### <a name="C.s2"></a>choice
```
"definition": {
	"description": {
		"en-US": "Which of these prototypes are available at the beta site?"
	},
	"type": "http://adlnet.gov/expapi/activities/cmi.interaction",
	"interactionType": "choice",
	"correctResponsesPattern": [
		"golf[,]tetris"
	],
	"choices": [
		{
			"id": "golf", 
			"description": {
				"en-US": "Golf Example"
			}
		},
		{
			"id": "facebook", 
			"description": {
				"en-US": "Facebook App"
			}
		},
		{
			"id": "tetris", 
			"description": {
				"en-US": "Tetris Example"
			}
		},
		{
			"id": "scrabble", 
			"description": {
				"en-US": "Scrabble Example"
			}
		}
	]
}
```

###### <a name="C.s3"></a>fill-in
```
"definition": {
	"description": {
		"en-US": "Ben is often heard saying: "
	},
	"type": "http://adlnet.gov/expapi/activities/cmi.interaction",
	"interactionType": "fill-in",
	"correctResponsesPattern": [
		"Bob's your uncle"
	]
}
```

###### <a name="C.s4"></a>long-fill-in
```
"definition": {
	"description": {
		"en-US": "What is the purpose of the xAPI?"
	},
	"type": "http://adlnet.gov/expapi/activities/cmi.interaction",
	"interactionType": "long-fill-in",
	"correctResponsesPattern": [
		"{case_matters=false}{lang=en}To store and provide access to learning experiences."
	]
}
```

###### <a name="C.s5"></a>likert
```
"definition": {
	"description": {
		"en-US": "How awesome is Experience API?"
	},
	"type": "http://adlnet.gov/expapi/activities/cmi.interaction",
	"interactionType": "likert",
	"correctResponsesPattern": [
		"likert_3"
	],
	"scale": [
		{
			"id": "likert_0", 
			"description": {
				"en-US": "It's OK"
			}
		},
		{
			"id": "likert_1", 
			"description": {
				"en-US": "It's Pretty Cool"
			}
		},
		{
			"id": "likert_2", 
			"description": {
				"en-US": "It's Damn Cool"
			}
		},
		{
			"id": "likert_3", 
			"description": {
				"en-US": "It's Gonna Change the World"
			}
		}
	]
}
```

###### <a name="C.s6"></a>matching
```
"definition": {
	"description": {
		"en-US": "Match these people to their kickball team:"
	},
	"type": "http://adlnet.gov/expapi/activities/cmi.interaction",
	"interactionType": "matching",
	"correctResponsesPattern": [
		"ben[.]3[,]chris[.]2[,]troy[.]4[,]freddie[.]1"
	],
	"source": [
		{
			"id": "ben",
			"description": {
				"en-US": "Ben"
			}
		},
		{
			"id": "chris",
			"description": {
				"en-US": "Chris"
			}
		},
		{
			"id": "troy",
			"description": {
				"en-US": "Troy"
			}
		},
		{
			"id": "freddie",
			"description": {
				"en-US": "Freddie"
			}
		}
	],
	"target": [
		{
			"id": "1",
			"description": {
				"en-US": "Swift Kick in the Grass"
			}
		},
		{
			"id": "2",
			"description": {
				"en-US": "We got Runs"
			}
		},
		{
			"id": "3",
			"description": {
				"en-US": "Duck"
			}
		},
		{
			"id": "4",
			"description": {
				"en-US": "Van Delay Industries"
			}
		}
	]
}
```

###### <a name="C.s7"></a>performance
```
"definition": {
	"description": {
		"en-US": "This interaction measures performance over a day of RS sports:"
	},
	"type": "http://adlnet.gov/expapi/activities/cmi.interaction",
	"interactionType": "performance",
	"correctResponsesPattern": [
		"pong[.]1:[,]dg[.]:10[,]lunch[.]"
	],
	"steps": [
		{
			"id": "pong", 
			"description": {
				"en-US": "Net pong matches won"
			}
		},
		{
			"id": "dg", 
			"description": {
				"en-US": "Strokes over par in disc golf at Liberty"
				}
			},
		{
			"id": "lunch", 
			"description": {
				"en-US": "Lunch having been eaten"
			}
		}
	]
}
```

###### <a name="C.s8"></a>sequencing
```
"definition": {
	"description": {
		"en-US": "Order players by their pong ladder position:"
	},
	"type": "http://adlnet.gov/expapi/activities/cmi.interaction",
	"interactionType": "sequencing",
	"correctResponsesPattern": [
		"tim[,]mike[,]ells[,]ben"
	],
	"choices": [
		{
			"id": "tim", 
			"description": {
				"en-US": "Tim"
			}
		},
		{
			"id": "ben", "description": {
				"en-US": "Ben"
			}
		},
		{
			"id": "ells", 
			"description": {
				"en-US": "Ells"
			}
		},
		{
			"id": "mike", 
			"description": {
				"en-US": "Mike"
			}
		}
	]
}
```

###### <a name="C.s9"></a>numeric
```
"definition": {
	"description": {
		"en-US": "How many jokes is Chris the butt of each day?"
	},
	"type": "http://adlnet.gov/expapi/activities/cmi.interaction",
	"interactionType": "numeric",
	"correctResponsesPattern": [
		"4[:]"
	]
}
```

In this example the minimum correct answer is `4` and there is no maximum. `5`, `6` or `976` would all be correct answers. 

###### <a name="C.s10"></a>other
```
"definition": {
	"description": {
		"en-US": "On this map, please mark Franklin, TN"
	},
	"type": "http://adlnet.gov/expapi/activities/cmi.interaction",
	"interactionType": "other",
	"correctResponsesPattern": [
		"(35.937432,-86.868896)"
	]
}
```

<a name="Appendix2D"/>

### <a name="D">Appendix D</a>: Example Signed Statement

An example signed Statement, as described in: [Section 2.6 Signed Statements](#signature).

The original Statement serialization to be signed. New lines in this example are included
via CR+LF (0x0D + 0x0A).

```
{
    "version": "1.0.0",
    "id": "33cff416-e331-4c9d-969e-5373a1756120",
    "actor": {
        "mbox": "mailto:example@example.com",
        "name": "Example Learner",
        "objectType": "Agent"
    },
    "verb": {
        "id": "http://adlnet.gov/expapi/verbs/experienced",
        "display": {
            "en-US": "experienced"
        }
    },
    "object": {
        "id": "https://www.youtube.com/watch?v=xh4kIiH3Sm8",
        "objectType": "Activity",
        "definition": {
            "name": {
                "en-US": "Tax Tips & Information : How to File a Tax Return "
            },
            "description": {
                "en-US": "Filing a tax return will require filling out either a 1040, 1040A or 1040EZ form"
            }
        }
    },
    "timestamp": "2013-04-01T12:00:00Z"
}
```

Example private key for X.509 certificate that will be used for signing:
```
-----BEGIN RSA PRIVATE KEY-----
MIICXAIBAAKBgQDjxvZXF30WL4oKjZYXgR0ZyaX+u3y6+JqTqiNkFa/VTnet6Ly2
OT6ZmmcJEPnq3UnewpHoOQ+GfhhTkW13j06j5iNn4obcCVWTL9yXNvJH+Ko+xu4Y
l/ySPRrIPyTjtHdG0M2XzIlmmLqm+CAS+KCbJeH4tf543kIWC5pC5p3cVQIDAQAB
AoGAOejdvGq2XKuddu1kWXl0Aphn4YmdPpPyCNTaxplU6PBYMRjY0aNgLQE6bO2p
/HJiU4Y4PkgzkEgCu0xf/mOq5DnSkX32ICoQS6jChABAe20ErPfm5t8h9YKsTfn9
40lAouuwD9ePRteizd4YvHtiMMwmh5PtUoCbqLefawNApAECQQD1mdBW3zL0okUx
2pc4tttn2qArCG4CsEZMLlGRDd3FwPWJz3ZPNEEgZWXGSpA9F1QTZ6JYXIfejjRo
UuvRMWeBAkEA7WvzDBNcv4N+xeUKvH8ILti/BM58LraTtqJlzjQSovek0srxtmDg
5of+xrxN6IM4p7yvQa+7YOUOukrVXjG+1QJBAI2mBrjzxgm9xTa5odn97JD7UMFA
/WHjlMe/Nx/35V52qaav1sZbluw+TvKMcqApYj5G2SUpSNudHLDGkmd2nQECQFfc
lBRK8g7ZncekbGW3aRLVGVOxClnLLTzwOlamBKOUm8V6XxsMHQ6TE2D+fKJoNUY1
2HGpk+FWwy2D1hRGuoUCQAXfaLSxtaWdPtlZTPVueF7ZikQDsVg+vtTFgpuHloR2
6EVc1RbHHZm32yvGDY8IkcoMfJQqLONDdLfS/05yoNU=
-----END RSA PRIVATE KEY-----
```

Example public X.509 certificate
```
-----BEGIN CERTIFICATE-----
MIIDATCCAmqgAwIBAgIJAMB1csNuA6+kMA0GCSqGSIb3DQEBBQUAMHExCzAJBgNV
BAYTAlVTMRIwEAYDVQQIEwlUZW5uZXNzZWUxGDAWBgNVBAoTD0V4YW1wbGUgQ29t
cGFueTEQMA4GA1UEAxMHRXhhbXBsZTEiMCAGCSqGSIb3DQEJARYTZXhhbXBsZUBl
eGFtcGxlLmNvbTAeFw0xMzA0MDQxNTI4MzBaFw0xNDA0MDQxNTI4MzBaMIGWMQsw
CQYDVQQGEwJVUzESMBAGA1UECBMJVGVubmVzc2VlMREwDwYDVQQHEwhGcmFua2xp
bjEYMBYGA1UEChMPRXhhbXBsZSBDb21wYW55MRAwDgYDVQQLEwdFeGFtcGxlMRAw
DgYDVQQDEwdFeGFtcGxlMSIwIAYJKoZIhvcNAQkBFhNleGFtcGxlQGV4YW1wbGUu
Y29tMIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDjxvZXF30WL4oKjZYXgR0Z
yaX+u3y6+JqTqiNkFa/VTnet6Ly2OT6ZmmcJEPnq3UnewpHoOQ+GfhhTkW13j06j
5iNn4obcCVWTL9yXNvJH+Ko+xu4Yl/ySPRrIPyTjtHdG0M2XzIlmmLqm+CAS+KCb
JeH4tf543kIWC5pC5p3cVQIDAQABo3sweTAJBgNVHRMEAjAAMCwGCWCGSAGG+EIB
DQQfFh1PcGVuU1NMIEdlbmVyYXRlZCBDZXJ0aWZpY2F0ZTAdBgNVHQ4EFgQUVs3v
5afEdOeoYeVajAQE4v0WS1QwHwYDVR0jBBgwFoAUyVIc3yvra4EBz20I4BF39IAi
xBkwDQYJKoZIhvcNAQEFBQADgYEAgS/FF5D0Hnj44rvT6kgn3kJAvv2lj/fyjztK
IrYS33ljXGn6gGyA4qtbXA23PrO4uc/wYCSDICDpPobh62xTCd9qObKhgwWOi05P
SBLqUu3mwfAe15LJBJBqPVZ4K0kppePBU8m6aIZoH57L/9t4OoaL8yKs/qjKFeI1
OFWZxvA=
-----END CERTIFICATE-----
```

Example certificate authority certificate
```
-----BEGIN CERTIFICATE-----
MIIDNzCCAqCgAwIBAgIJAMB1csNuA6+jMA0GCSqGSIb3DQEBBQUAMHExCzAJBgNV
BAYTAlVTMRIwEAYDVQQIEwlUZW5uZXNzZWUxGDAWBgNVBAoTD0V4YW1wbGUgQ29t
cGFueTEQMA4GA1UEAxMHRXhhbXBsZTEiMCAGCSqGSIb3DQEJARYTZXhhbXBsZUBl
eGFtcGxlLmNvbTAeFw0xMzA0MDQxNTI1NTNaFw0yMzA0MDIxNTI1NTNaMHExCzAJ
BgNVBAYTAlVTMRIwEAYDVQQIEwlUZW5uZXNzZWUxGDAWBgNVBAoTD0V4YW1wbGUg
Q29tcGFueTEQMA4GA1UEAxMHRXhhbXBsZTEiMCAGCSqGSIb3DQEJARYTZXhhbXBs
ZUBleGFtcGxlLmNvbTCBnzANBgkqhkiG9w0BAQEFAAOBjQAwgYkCgYEA1sBnBWPZ
0f7WJUFTJy5+01SlS5Z6DDD6Uye9vK9AycgV5B3+WC8HC5u5h91MujAC1ARPVUOt
svPRs45qKNFIgIGRXKPAwZjawEI2sCJRSKV47i6B8bDv4WkuGvQaveZGI0qlmN5R
1Eim2gUItRj1hgcC9rQavjlnFKDY2rlXGukCAwEAAaOB1jCB0zAdBgNVHQ4EFgQU
yVIc3yvra4EBz20I4BF39IAixBkwgaMGA1UdIwSBmzCBmIAUyVIc3yvra4EBz20I
4BF39IAixBmhdaRzMHExCzAJBgNVBAYTAlVTMRIwEAYDVQQIEwlUZW5uZXNzZWUx
GDAWBgNVBAoTD0V4YW1wbGUgQ29tcGFueTEQMA4GA1UEAxMHRXhhbXBsZTEiMCAG
CSqGSIb3DQEJARYTZXhhbXBsZUBleGFtcGxlLmNvbYIJAMB1csNuA6+jMAwGA1Ud
EwQFMAMBAf8wDQYJKoZIhvcNAQEFBQADgYEADhwTebGk735yKhm8DqCxvNnEZ0Nx
sYEYOjgRG1yXTlW5pE691fSH5AZ+T6fpwpZcWY5QYkoN6DnwjOxGkSfQC3/yGmcU
DKBPwiZ5O2s9C+fE1kUEnrX2Xea4agVngMzR8DQ6oOauLWqehDB+g2ENWRLoVgS+
ma5/Ycs0GTyrECY=
-----END CERTIFICATE-----
```

JWS Header. Note that along with specifying the algorithm, the certificate chain for
the signing certificate has been included.
```
{
    "alg": "RS256",
    "x5c": [
        "MIIDATCCAmqgAwIBAgIJAMB1csNuA6+kMA0GCSqGSIb3DQEBBQUAMHExCzAJBgNVBAYTAlVTMRIwEAYDVQQIEwlUZW5uZXNzZWUxGDAWBgNVBAoTD0V4YW1wbGUgQ29tcGFueTEQMA4GA1UEAxMHRXhhbXBsZTEiMCAGCSqGSIb3DQEJARYTZXhhbXBsZUBleGFtcGxlLmNvbTAeFw0xMzA0MDQxNTI4MzBaFw0xNDA0MDQxNTI4MzBaMIGWMQswCQYDVQQGEwJVUzESMBAGA1UECBMJVGVubmVzc2VlMREwDwYDVQQHEwhGcmFua2xpbjEYMBYGA1UEChMPRXhhbXBsZSBDb21wYW55MRAwDgYDVQQLEwdFeGFtcGxlMRAwDgYDVQQDEwdFeGFtcGxlMSIwIAYJKoZIhvcNAQkBFhNleGFtcGxlQGV4YW1wbGUuY29tMIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDjxvZXF30WL4oKjZYXgR0ZyaX+u3y6+JqTqiNkFa/VTnet6Ly2OT6ZmmcJEPnq3UnewpHoOQ+GfhhTkW13j06j5iNn4obcCVWTL9yXNvJH+Ko+xu4Yl/ySPRrIPyTjtHdG0M2XzIlmmLqm+CAS+KCbJeH4tf543kIWC5pC5p3cVQIDAQABo3sweTAJBgNVHRMEAjAAMCwGCWCGSAGG+EIBDQQfFh1PcGVuU1NMIEdlbmVyYXRlZCBDZXJ0aWZpY2F0ZTAdBgNVHQ4EFgQUVs3v5afEdOeoYeVajAQE4v0WS1QwHwYDVR0jBBgwFoAUyVIc3yvra4EBz20I4BF39IAixBkwDQYJKoZIhvcNAQEFBQADgYEAgS/FF5D0Hnj44rvT6kgn3kJAvv2lj/fyjztKIrYS33ljXGn6gGyA4qtbXA23PrO4uc/wYCSDICDpPobh62xTCd9qObKhgwWOi05PSBLqUu3mwfAe15LJBJBqPVZ4K0kppePBU8m6aIZoH57L/9t4OoaL8yKs/qjKFeI1OFWZxvA=",
        "MIIDNzCCAqCgAwIBAgIJAMB1csNuA6+jMA0GCSqGSIb3DQEBBQUAMHExCzAJBgNVBAYTAlVTMRIwEAYDVQQIEwlUZW5uZXNzZWUxGDAWBgNVBAoTD0V4YW1wbGUgQ29tcGFueTEQMA4GA1UEAxMHRXhhbXBsZTEiMCAGCSqGSIb3DQEJARYTZXhhbXBsZUBleGFtcGxlLmNvbTAeFw0xMzA0MDQxNTI1NTNaFw0yMzA0MDIxNTI1NTNaMHExCzAJBgNVBAYTAlVTMRIwEAYDVQQIEwlUZW5uZXNzZWUxGDAWBgNVBAoTD0V4YW1wbGUgQ29tcGFueTEQMA4GA1UEAxMHRXhhbXBsZTEiMCAGCSqGSIb3DQEJARYTZXhhbXBsZUBleGFtcGxlLmNvbTCBnzANBgkqhkiG9w0BAQEFAAOBjQAwgYkCgYEA1sBnBWPZ0f7WJUFTJy5+01SlS5Z6DDD6Uye9vK9AycgV5B3+WC8HC5u5h91MujAC1ARPVUOtsvPRs45qKNFIgIGRXKPAwZjawEI2sCJRSKV47i6B8bDv4WkuGvQaveZGI0qlmN5R1Eim2gUItRj1hgcC9rQavjlnFKDY2rlXGukCAwEAAaOB1jCB0zAdBgNVHQ4EFgQUyVIc3yvra4EBz20I4BF39IAixBkwgaMGA1UdIwSBmzCBmIAUyVIc3yvra4EBz20I4BF39IAixBmhdaRzMHExCzAJBgNVBAYTAlVTMRIwEAYDVQQIEwlUZW5uZXNzZWUxGDAWBgNVBAoTD0V4YW1wbGUgQ29tcGFueTEQMA4GA1UEAxMHRXhhbXBsZTEiMCAGCSqGSIb3DQEJARYTZXhhbXBsZUBleGFtcGxlLmNvbYIJAMB1csNuA6+jMAwGA1UdEwQFMAMBAf8wDQYJKoZIhvcNAQEFBQADgYEADhwTebGk735yKhm8DqCxvNnEZ0NxsYEYOjgRG1yXTlW5pE691fSH5AZ+T6fpwpZcWY5QYkoN6DnwjOxGkSfQC3/yGmcUDKBPwiZ5O2s9C+fE1kUEnrX2Xea4agVngMzR8DQ6oOauLWqehDB+g2ENWRLoVgS+ma5/Ycs0GTyrECY="
    ]
}
```

JWS signature
```
ew0KICAgICJhbGciOiAiUlMyNTYiLA0KICAgICJ4NWMiOiBbDQogICAgICAgICJNSUlEQVRDQ0FtcWdBd0lCQWdJSkFNQjFjc051QTYra01BMEdDU3FHU0liM0RRRUJCUVVBTUhFeEN6QUpCZ05WQkFZVEFsVlRNUkl3RUFZRFZRUUlFd2xVWlc1dVpYTnpaV1V4R0RBV0JnTlZCQW9URDBWNFlXMXdiR1VnUTI5dGNHRnVlVEVRTUE0R0ExVUVBeE1IUlhoaGJYQnNaVEVpTUNBR0NTcUdTSWIzRFFFSkFSWVRaWGhoYlhCc1pVQmxlR0Z0Y0d4bExtTnZiVEFlRncweE16QTBNRFF4TlRJNE16QmFGdzB4TkRBME1EUXhOVEk0TXpCYU1JR1dNUXN3Q1FZRFZRUUdFd0pWVXpFU01CQUdBMVVFQ0JNSlZHVnVibVZ6YzJWbE1SRXdEd1lEVlFRSEV3aEdjbUZ1YTJ4cGJqRVlNQllHQTFVRUNoTVBSWGhoYlhCc1pTQkRiMjF3WVc1NU1SQXdEZ1lEVlFRTEV3ZEZlR0Z0Y0d4bE1SQXdEZ1lEVlFRREV3ZEZlR0Z0Y0d4bE1TSXdJQVlKS29aSWh2Y05BUWtCRmhObGVHRnRjR3hsUUdWNFlXMXdiR1V1WTI5dE1JR2ZNQTBHQ1NxR1NJYjNEUUVCQVFVQUE0R05BRENCaVFLQmdRRGp4dlpYRjMwV0w0b0tqWllYZ1IwWnlhWCt1M3k2K0pxVHFpTmtGYS9WVG5ldDZMeTJPVDZabW1jSkVQbnEzVW5ld3BIb09RK0dmaGhUa1cxM2owNmo1aU5uNG9iY0NWV1RMOXlYTnZKSCtLbyt4dTRZbC95U1BScklQeVRqdEhkRzBNMlh6SWxtbUxxbStDQVMrS0NiSmVINHRmNTQza0lXQzVwQzVwM2NWUUlEQVFBQm8zc3dlVEFKQmdOVkhSTUVBakFBTUN3R0NXQ0dTQUdHK0VJQkRRUWZGaDFQY0dWdVUxTk1JRWRsYm1WeVlYUmxaQ0JEWlhKMGFXWnBZMkYwWlRBZEJnTlZIUTRFRmdRVVZzM3Y1YWZFZE9lb1llVmFqQVFFNHYwV1MxUXdId1lEVlIwakJCZ3dGb0FVeVZJYzN5dnJhNEVCejIwSTRCRjM5SUFpeEJrd0RRWUpLb1pJaHZjTkFRRUZCUUFEZ1lFQWdTL0ZGNUQwSG5qNDRydlQ2a2duM2tKQXZ2MmxqL2Z5anp0S0lyWVMzM2xqWEduNmdHeUE0cXRiWEEyM1ByTzR1Yy93WUNTRElDRHBQb2JoNjJ4VENkOXFPYktoZ3dXT2kwNVBTQkxxVXUzbXdmQWUxNUxKQkpCcVBWWjRLMGtwcGVQQlU4bTZhSVpvSDU3TC85dDRPb2FMOHlLcy9xaktGZUkxT0ZXWnh2QT0iLA0KICAgICAgICAiTUlJRE56Q0NBcUNnQXdJQkFnSUpBTUIxY3NOdUE2K2pNQTBHQ1NxR1NJYjNEUUVCQlFVQU1IRXhDekFKQmdOVkJBWVRBbFZUTVJJd0VBWURWUVFJRXdsVVpXNXVaWE56WldVeEdEQVdCZ05WQkFvVEQwVjRZVzF3YkdVZ1EyOXRjR0Z1ZVRFUU1BNEdBMVVFQXhNSFJYaGhiWEJzWlRFaU1DQUdDU3FHU0liM0RRRUpBUllUWlhoaGJYQnNaVUJsZUdGdGNHeGxMbU52YlRBZUZ3MHhNekEwTURReE5USTFOVE5hRncweU16QTBNREl4TlRJMU5UTmFNSEV4Q3pBSkJnTlZCQVlUQWxWVE1SSXdFQVlEVlFRSUV3bFVaVzV1WlhOelpXVXhHREFXQmdOVkJBb1REMFY0WVcxd2JHVWdRMjl0Y0dGdWVURVFNQTRHQTFVRUF4TUhSWGhoYlhCc1pURWlNQ0FHQ1NxR1NJYjNEUUVKQVJZVFpYaGhiWEJzWlVCbGVHRnRjR3hsTG1OdmJUQ0JuekFOQmdrcWhraUc5dzBCQVFFRkFBT0JqUUF3Z1lrQ2dZRUExc0JuQldQWjBmN1dKVUZUSnk1KzAxU2xTNVo2RERENlV5ZTl2SzlBeWNnVjVCMytXQzhIQzV1NWg5MU11akFDMUFSUFZVT3RzdlBSczQ1cUtORklnSUdSWEtQQXdaamF3RUkyc0NKUlNLVjQ3aTZCOGJEdjRXa3VHdlFhdmVaR0kwcWxtTjVSMUVpbTJnVUl0UmoxaGdjQzlyUWF2amxuRktEWTJybFhHdWtDQXdFQUFhT0IxakNCMHpBZEJnTlZIUTRFRmdRVXlWSWMzeXZyYTRFQnoyMEk0QkYzOUlBaXhCa3dnYU1HQTFVZEl3U0JtekNCbUlBVXlWSWMzeXZyYTRFQnoyMEk0QkYzOUlBaXhCbWhkYVJ6TUhFeEN6QUpCZ05WQkFZVEFsVlRNUkl3RUFZRFZRUUlFd2xVWlc1dVpYTnpaV1V4R0RBV0JnTlZCQW9URDBWNFlXMXdiR1VnUTI5dGNHRnVlVEVRTUE0R0ExVUVBeE1IUlhoaGJYQnNaVEVpTUNBR0NTcUdTSWIzRFFFSkFSWVRaWGhoYlhCc1pVQmxlR0Z0Y0d4bExtTnZiWUlKQU1CMWNzTnVBNitqTUF3R0ExVWRFd1FGTUFNQkFmOHdEUVlKS29aSWh2Y05BUUVGQlFBRGdZRUFEaHdUZWJHazczNXlLaG04RHFDeHZObkVaME54c1lFWU9qZ1JHMXlYVGxXNXBFNjkxZlNINUFaK1Q2ZnB3cFpjV1k1UVlrb042RG53ak94R2tTZlFDMy95R21jVURLQlB3aVo1TzJzOUMrZkUxa1VFbnJYMlhlYTRhZ1ZuZ016UjhEUTZvT2F1TFdxZWhEQitnMkVOV1JMb1ZnUyttYTUvWWNzMEdUeXJFQ1k9Ig0KICAgIF0NCn0.ew0KICAgICJ2ZXJzaW9uIjogIjEuMC4wIiwNCiAgICAiaWQiOiAiMzNjZmY0MTYtZTMzMS00YzlkLTk2OWUtNTM3M2ExNzU2MTIwIiwNCiAgICAiYWN0b3IiOiB7DQogICAgICAgICJtYm94IjogIm1haWx0bzpleGFtcGxlQGV4YW1wbGUuY29tIiwNCiAgICAgICAgIm5hbWUiOiAiRXhhbXBsZSBMZWFybmVyIiwNCiAgICAgICAgIm9iamVjdFR5cGUiOiAiQWdlbnQiDQogICAgfSwNCiAgICAidmVyYiI6IHsNCiAgICAgICAgImlkIjogImh0dHA6Ly9hZGxuZXQuZ292L2V4cGFwaS92ZXJicy9leHBlcmllbmNlZCIsDQogICAgICAgICJkaXNwbGF5Ijogew0KICAgICAgICAgICAgImVuLVVTIjogImV4cGVyaWVuY2VkIg0KICAgICAgICB9DQogICAgfSwNCiAgICAib2JqZWN0Ijogew0KICAgICAgICAiaWQiOiAiaHR0cHM6Ly93d3cueW91dHViZS5jb20vd2F0Y2g_dj14aDRrSWlIM1NtOCIsDQogICAgICAgICJvYmplY3RUeXBlIjogIkFjdGl2aXR5IiwNCiAgICAgICAgImRlZmluaXRpb24iOiB7DQogICAgICAgICAgICAibmFtZSI6IHsNCiAgICAgICAgICAgICAgICAiZW4tVVMiOiAiVGF4IFRpcHMgJiBJbmZvcm1hdGlvbiA6IEhvdyB0byBGaWxlIGEgVGF4IFJldHVybiAiDQogICAgICAgICAgICB9LA0KICAgICAgICAgICAgImRlc2NyaXB0aW9uIjogew0KICAgICAgICAgICAgICAgICJlbi1VUyI6ICJGaWxpbmcgYSB0YXggcmV0dXJuIHdpbGwgcmVxdWlyZSBmaWxsaW5nIG91dCBlaXRoZXIgYSAxMDQwLCAxMDQwQSBvciAxMDQwRVogZm9ybSINCiAgICAgICAgICAgIH0NCiAgICAgICAgfQ0KICAgIH0sDQogICAgInRpbWVzdGFtcCI6ICIyMDEzLTA0LTAxVDEyOjAwOjAwWiINCn0.FWuwaPhwUbkk7h9sKW5zSvjsYNugvxJ-TrVaEgt_DCUT0bmKhQScRrjMB6P9O50uznPwT66oF1NnU_G0HVhRzS5voiXE-y7tT3z0M3-8A6YK009Bk_digVUul-HA4Fpd5IjoBBGe3yzaQ2ZvzarvRuipvNEQCI0onpfuZZJQ0d8
```

Signed Statement
```
{
    "version": "1.0.0",
    "id": "33cff416-e331-4c9d-969e-5373a1756120",
    "actor": {
        "mbox": "mailto:example@example.com",
        "name": "Example Learner",
        "objectType": "Agent"
    },
    "verb": {
        "id": "http://adlnet.gov/expapi/verbs/experienced",
        "display": {
            "en-US": "experienced"
        }
    },
    "object": {
        "id": "https://www.youtube.com/watch?v=xh4kIiH3Sm8",
        "objectType": "Activity",
        "definition": {
            "name": {
                "en-US": "Tax Tips & Information : How to File a Tax Return "
            },
            "description": {
                "en-US": "Filing a tax return will require filling out either a 1040, 1040A or 1040EZ form"
            }
        }
    },
    "timestamp": "2013-04-01T12:00:00Z",
    "attachments": [
        {
            "usageType": "http://adlnet.gov/expapi/attachments/signature",
            "display": { "en-US": "Signature" },
            "description": { "en-US": "A test signature" },
            "contentType": "application/octet-stream",
            "length": 4235,
            "sha2": "672fa5fa658017f1b72d65036f13379c6ab05d4ab3b6664908d8acf0b6a0c634"
        }
    ]
}
```

__Note:__ Attached signature not shown, see [Attachments](#attachments) for Attachment message format.

