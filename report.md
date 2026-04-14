#!/bin/bash

NOTES_DIR="../../notes"
DATA_DIR="../../data"

mkdir -p "$NOTES_DIR"

TODAY=$(date +"%Y-%m-%d")

REPORT_FILE="$NOTES_DIR/report_$TODAY.txt"

USER_NAME=$(whoami)
CURRENT_PATH=$(pwd)

if [ -d "$DATA_DIR" ]; then
    FILE_COUNT=$(find "$DATA_DIR" -type f | wc -l)
else
    FILE_COUNT=0
fi

cat <<EOF > "$REPORT_FILE"
تقرير يومي - $TODAY

اسم المستخدم: $USER_NAME
المسار الحالي: $CURRENT_PATH
عدد الملفات داخل data: $FILE_COUNT
EOF

echo "تم إنشاء التقرير بنجاح ✔️"
