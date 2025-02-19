---

copyright:

  years: 2015, 2019

lastupdated: "2019-05-16"

keywords: help managing cases, resolve issues managing cases, trouble working with cases

subcollection: get-support

---


{:tsSymptoms: .tsSymptoms}
{:tsCauses: .tsCauses}
{:tsResolve: .tsResolve}
{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:new_window: target="_blank"}


# 管理支援案例的疑難排解
{: #Supportcases}

建立及管理 {{site.data.keyword.Bluemix}} 支援案例時，可能會發生問題。在許多情況下，您可以遵照一些簡單的步驟，從這些問題回復。
{:shortdesc}

## 為什麼我無法建立或編輯支援案例？ 
{: #ts_service_broker}

您無法建立或編輯 {{site.data.keyword.Bluemix_notm}} 支援案例，並且收到您沒有適當存取權的錯誤訊息。
{:shortdesc}

當您嘗試建立案例時，會顯示下列錯誤訊息：   
{: tsSymptoms}

`您似乎沒有存取權以建立此帳戶的案例。`

存取及管理支援案例的一般問題，可能是因為沒有「支援中心」帳戶管理服務的 Identity and Access Management (IAM) 存取原則所致。您必須要獲得指派支援中心帳戶管理服務的編輯者或管理者角色，才能建立案例。
{: tsCauses}

為了解決問題，帳戶擁有者、支援中心服務的管理者，或是所有帳戶管理服務的管理者，可以指派支援中心的 IAM 原則以便管理案例。
{: tsResolve}

如果您是帳戶擁有者或「支援中心」的管理者，請完成下列步驟，以建立使用支援案例用的存取原則：

1. 移至**管理** &gt; **存取 (IAM)**，然後選取**使用者**。
2. 選取使用者名稱，然後按一下**存取原則**。 
3. 按一下**指派存取權**。 
4. 選取**指派對帳戶管理服務的存取權**。 
5. 從**服務**功能表，選取**支援中心**。 
6. 選取角色以定義使用者的存取層次。 


## 為什麼我無法檢視帳戶中的所有案例？
{: #ts_viewcasedetails}

您無法檢視帳戶中的所有案例，因為您沒有存取權，無法檢視帳戶中的所有使用者。
{:shortdesc}

當您嘗試檢視與帳戶相關聯的支援案例時，您無法看到所有開立的案例。
{: tsSymptoms}

帳戶擁有者將[使用者清單可見性設定](/docs/iam?topic=iam-userlistview#userlistview)設為受限。將設定設為受限時，如果您沒有其他存取原則可檢視帳戶中的使用者，則您不具備檢視帳戶中所有案例的必要存取權。您只能檢視您邀請加入帳戶的使用者、與其共用 Cloud Foundry 組織成員資格的使用者，或是處於您標準基礎架構使用者階層中的使用者。
{: tsCauses}

除了「支援中心」帳戶管理服務存取原則之外，您還必須獲指派至少具有「使用者管理」帳戶管理服務之「檢視者」角色的 IAM 原則。若要檢視現行存取權，請移至**管理** &gt; **存取 (IAM)**，然後從**使用者**頁面中選取您的名稱。按一下**存取原則**標籤，並檢閱已指派的原則。
{: tsResolve}

若要解決此問題，請與帳戶擁有者聯絡，以要求適當的存取權。 

## 為什麼我找不到先前建立的案例？ 
{: #ts_viewarchivedcase}

您找不到在加強 {{site.data.keyword.Bluemix_notm}} 平台體驗之前所建立的案例。
{:shortdesc}

在移至「支援中心」的**管理案例**標籤之後，您找不到在 2018 年 12 月 2 日之前建立的所有案例。
{: tsSymptoms}

2018 年 12 月 2 日之前開立的案例只能透過**檢視保存的案例**進行檢視。
{: tsCauses}

若要檢視您的案例，請移至**支援**，並選取**管理案例**，然後按一下**檢視保存的案例**。
{: tsResolve} 






