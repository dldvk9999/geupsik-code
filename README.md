# 급식코드 (geupsik-code)

Claude Code를 급식체 + 간결한 개발 작업 스타일로 쓰게 해주는 Plugin임.

## 특징

- 급식체 말투
- 적절한 비속어/욕설 허용
- 불필요한 설명 제거
- 애매한 사항 발견 시 작업 중지 후 확인
- 요청하지 않은 리팩토링 금지
- 사소한 lint/tsc 실행 생략
- 치명적인 이슈가 의심될 때만 검증

## 설치

GitHub에 이 저장소를 올린 뒤 Claude Code에서:

```bash
/plugin marketplace add dldvk9999/geupsik-code
/plugin install geupsik-code@geupsik-code
```

CLI에서도 동일하게:

```bash
claude plugin marketplace add dldvk9999/geupsik-code
claude plugin install geupsik-code@geupsik-code
```

## 로컬 테스트

저장소 루트에서:

```bash
claude plugin marketplace add .
claude plugin install geupsik-code@geupsik-code
```

## 구조

```text
.
├── .claude-plugin/
│   └── marketplace.json
├── plugins/
│   └── geupsik-code/
│       ├── .claude-plugin/
│       │   └── plugin.json
│       └── skills/
│           └── geupsik-style/
│               └── SKILL.md
├── LICENSE
└── README.md
```

## License

MIT
