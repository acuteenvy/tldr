# bfs

> 파일에 대한 너비 우선 검색.
> 더 많은 정보: <https://manned.org/bfs>.

- 확장자로 파일 찾기:

`bfs {{루트_경로}} -name '{{*.ext}}'`

- 여러 경로/이름 패턴과 일치하는 파일 찾기:

`bfs {{루트_경로}} -path '{{**/경로/**/*.ext}}' -or -name '{{*패턴*}}'`

- 대소문자를 구분하지 않는 모드에서, 주어진 이름과 일치하는 디렉터리를 찾음:

`bfs {{루트_경로}} -type d -iname '{{*lib*}}'`

- 특정 경로를 제외하고 주어진 패턴과 일치하는 파일을 찾음:

`bfs {{루트_경로}} -name '{{*.py}}' -not -path '{{*/사이트-패키지/*}}'`

- 재귀 깊이를 "1"로 제한하여 지정된 크기 범위와 일치하는 파일을 찾음:

`bfs {{루트_경로}} -maxdepth 1 -size {{+500k}} -size {{-10M}}`

- 각 파일에 대해 명령을 실행 (파일 이름에 접근하려면 명령 내에서 `{}` 사용):

`bfs {{루트_경로}} -name '{{*.ext}}' -exec {{wc -l}} {} \;`

- 오늘 수정된 모든 파일을 찾아, 결과를 단일 명령에 인수로 전달:

`bfs {{루트_경로}} -daystart -mtime {{-1}} -exec {{tar -cvf archive.tar}} {} \+`

- 빈 파일 (0 바이트) 또는 디렉터리를 찾아 상세하게 삭제:

`bfs {{루트_경로}} -type {{f|d}} -empty -delete -print`
