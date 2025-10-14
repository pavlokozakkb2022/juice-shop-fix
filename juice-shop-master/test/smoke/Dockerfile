FROM alpine

RUN adduser -D appuser

RUN apk add curl

USER appuser

COPY --chown=appuser:appuser smoke-test.sh smoke-test.sh

CMD ["sh", "smoke-test.sh", "http://app:3000"]