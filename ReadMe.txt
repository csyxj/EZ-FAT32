������FAT32�ļ�ϵͳ�������У���ȡ�ļ����У����������ļ����У������ļ���д�����ݡ�

���ϲ��ṩ��API����������FATFS.H�У����£�
FS_Status   Search_inDir(FS_Object *CurDir, FS_Object *Target, u8 *Target_Name, u8 Object);
u8         *ReadFile(FS_Object *Target_File);
void        SetFileClustoFst(FS_Object *Target_File);
FS_Status   OpenFile(FS_Object *Target, u8 *FullName);
void        LsDir(FS_Object *CurDir);

FS_Status   CreateNewObject(FS_Object *CurDir, FS_Object *Target, u8 *Target_Name, u8 Object);
void        WriteFile(FS_Object *Target_File, u8 *dataBuf, u32 dataLength);

��ֲʱ��ʵ�ֵĵײ�ӿں�����Interface.C�С��������£�
void Disk_ReadSec(u32 Addr, u32 *DataBuf);

void Disk_WriteSec(u32 Addr, u32 *DataBuf);


u16 UnicodeToGb2312(u16 Unicode);