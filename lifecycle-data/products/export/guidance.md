---
title: 수명 주기 데이터 내보내기 지침
description: 제품 수명 주기 정보 내보내기 지침
ms.date: 12/16/2020
layout: ContentPage
ms.openlocfilehash: 5e9dddbff5fac32e6d3cf8ef0943151d2dfe5e35
ms.sourcegitcommit: 6ea3221fd5475440480515f04f33988656d71748
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/02/2021
ms.locfileid: "3546862"
---
# <a name="lifecycle-data-export-guidance"></a>수명 주기 데이터 내보내기 지침
이 문서에서는 제품 내보내기 파일을 사용하는 방법을 설명합니다.

## <a name="query-information"></a>쿼리 정보
이 Excel 문서에는 제품 테이블에 채워진 데이터를 식별하는 데 도움이 되는 필드가 있습니다.

### <a name="end-of-support"></a>지원 종료
지원 종료 값은 제품 지원 종료 날짜 또는 릴리스 종료 날짜를 통해 제품을 필터링합니다.

가능한 값: All(필터가 적용되지 않음), Year, Range.

### <a name="family"></a>제품군
패밀리 값은 패밀리라고 하는 계층 구조 내의 상위 수준으로 제품을 필터링합니다.

가능한 값: All(필터가 적용되지 않음), Family Name

### <a name="group"></a>그룹
그룹 값은 상위 수준(패밀리) 내의 제품을 특정 그룹으로 필터링합니다.

가능한 값: All(필터가 적용되지 없음), Group Name

## <a name="table-columns"></a>표 열
제품 테이블은 제품, 버전, 릴리스 및 해당 지원 날짜를 정의하는 열로 구성됩니다.

> [!NOTE]
> 각 제품, 버전 및 릴리스 조합에 대해 행이 있습니다.

### <a name="product"></a>제품
제품 이름

### <a name="edition"></a>에디션
버전 열은 제품에 버전이 포함되어 있을 때 채워지며, 제품 버전이 없는 경우 이 필드는 비어 있습니다.

### <a name="release"></a>릴리스
제품에 여러 릴리스가 포함되어 있을 때 릴리스 열이 채워지게 됩니다.
제품에 릴리스가 하나만 있는 경우 이 필드는 비어 있습니다.

### <a name="support-policy"></a>지원 정책
이 필드는 제품이 따르는 지원 정책을 정의합니다.

가능한 값: [Fixed](/lifecycle/policies/fixed), [Modern](/lifecycle/policies/modern), Component

### <a name="start-date"></a>시작 날짜
제품에 대한 지원이 시작된 날짜입니다.

### <a name="mainstream-date"></a>기본 날짜
지원 정책이 **Fixed** 또는 **Component** 인 경우 이 날짜는 제품의 기본 종료 날짜입니다.
  
지원 정책이 **Modern** 이면 비어 있습니다.

### <a name="extended-end-date"></a>추가 지원 종료 날짜
지원 정책이 **Fixed** 또는 **Component** 인 경우 이 날짜는 제품의 연장된 종료 날짜입니다.

지원 정책이 **Modern** 이면 비어 있습니다.

### <a name="retirement-date"></a>사용 중지 날짜
지원 정책이 **고정** 또는 **Component** 인 경우 이 필드는 비어 있습니다.

지원 정책이 **Modern** 인 경우 제품의 사용 중지 날짜입니다.

### <a name="release-start-date"></a>릴리스 시작 날짜
해당 릴리스에 대한 지원이 시작된 날짜입니다. 제품에 릴리스가 하나만 있는 경우 이 필드는 비어 있습니다.
 
### <a name="release-end-date"></a>릴리스 종료 날짜
해당 릴리스에 대한 지원이 종료된 날짜입니다.
제품에 릴리스가 하나만 있는 경우 이 필드는 비어 있습니다.

### <a name="docs-url"></a>Docs Url
확장 설명서의 URL입니다.
