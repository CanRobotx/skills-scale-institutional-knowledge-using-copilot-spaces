# OctoAcme 프로젝트 관리 프로세스

## 개요

OctoAcme의 프로젝트 관리는 **고객 중심, 반복적 전달, 명확한 소유권, 데이터 기반 의사결정**의 핵심 원칙에 기반하고 있습니다. 프로젝트는 5단계 생명주기를 따릅니다: (1) 착수 단계에서 문제 진술과 이해관계자 확인, (2) 계획 단계에서 범위와 리스크 식별, (3) 실행 단계에서 빌드 및 검증, (4) 릴리스 단계에서 프로덕션 배포, (5) 종료 및 회고를 통한 학습 포착입니다. 각 프로젝트는 Project Manager(PM)와 Product Manager(PdM)의 명확한 이중 리더십 하에 진행되며, 개발자, QA, 이해관계자들과의 협력을 통해 고객 가치를 최대화합니다.

워크플로우는 GitHub Projects 기반의 프로젝트 보드(Backlog → Ready → In Progress → In Review → QA → Done)와 엄격한 Pull Request 규율을 중심으로 운영됩니다. 각 작업은 명확한 수용 기준과 정의된 완료 조건(DoD)을 갖추어야 하며, 소형 PR(≤400줄)로 분할하여 빠른 검토와 병합을 가능하게 합니다. 리스크는 ID, 설명, 영향도, 확률, 소유자, 완화 계획이 포함된 Risk Register에 체계적으로 기록되며, 주간 동기화 회의에서 모니터링됩니다. 의존성과 교차 팀 이슈는 프로젝트 보드에 명시되어 에스컬레이션 경로(팀 → PM → Product Lead → 스폰서)를 따릅니다.

품질 보증은 다층적 검증 프레임워크로 구현됩니다. 새로운 로직에 대한 단위 테스트, 필요시 통합 테스트, 그리고 릴리스 전 중요 흐름에 대한 엔드투엔드 스모크 테스트가 필수입니다. CI 파이프라인에 자동화된 테스트와 린팅, 보안 스캔이 통합되어 있으며, 모든 변경사항이 최소 1건의 승인 후 병합됩니다. 릴리스 전에는 배포 체크리스트를 통해 모든 수용 기준 충족, CI 통과, 보안 스캔 완료, 릴리스 노트 작성, 롤백 계획 수립을 확인합니다.

의사소통은 규칙적이고 구조화된 리듬으로 진행됩니다. 일일 스탠드업(15분)에서는 진행 상황, 차단 사항, 의존성에 집중하고, 주간 전달 동기화에서는 진전 상황과 플래그 처리된 리스크를 공유합니다. 주간 PM과 PdM 간의 정렬 회의, 월간 이해관계자 업데이트, 그리고 스프린트 또는 마일스톤 말미의 데모/검토 세션이 투명성과 정렬을 유지합니다. 주간 상태 템플릿(금주 진행 상황, 다음 단계, 리스크/차단 사항, 필요한 결정)과 사건 통신 프로토콜을 통해 일관된 정보 흐름을 보장하며, 회고를 통해 팀의 암묵적 지식을 명시적 개선 항목으로 전환합니다.

## 문서 목록

- [OctoAcme Project Management Overview](octoacme-project-management-overview.md)
- [OctoAcme — Project Initiation Guide](octoacme-project-initiation.md)
- [OctoAcme — Project Planning](octoacme-project-planning.md)
- [OctoAcme — Execution & Tracking](octoacme-execution-and-tracking.md)
- [OctoAcme — Risk Management & Communication](octoacme-risks-and-communication.md)
- [OctoAcme — Release & Deployment Guide](octoacme-release-and-deployment.md)
- [OctoAcme — Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
- [OctoAcme Personas](octoacme-roles-and-personas.md)
