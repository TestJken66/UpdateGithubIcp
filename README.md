# UpdateGithubIcp
run!!!

## 远程调用
``` shell
curl -X POST https://api.github.com/repos/:owner/:repo/dispatches \
    -H "Accept: application/vnd.github.everest-preview+json" \
    -H "Authorization: token TRIGGER_TOKEN" \
    --data '{"event_type": "TRIGGER_EVENT"}'

## 触发webhook-1
curl -X POST https://api.github.com/repos/TestJken66/UpdateGithubIcp/dispatches \
    -H "Accept: application/vnd.github.everest-preview+json" \
    -H "Authorization: token ghp_xxxxxxxxxxxxxxxxxxxxxxxxxx" \
    --data '{"event_type": "webhook-1"}'
    
####

curl -X POST https://api.github.com/repos/TestJken66/UpdateGithubIcp/dispatches \
    -H "Accept: application/vnd.github.everest-preview+json" \
    -H "Authorization: token $GTOKEN" \
    --data '{"event_type": "companys"}'

```
- https://docs.github.com/zh/actions/using-workflows/events-that-trigger-workflows