set(resource_url_base http://lotus.kuee.kyoto-u.ac.jp/~arseny/jumanpp_build)

file(DOWNLOAD ${resource_url_base}/testlm ${CMAKE_CURRENT_SOURCE_DIR}/rnn/testlm
        SHOW_PROGRESS EXPECTED_MD5 d492bc63778aaa7e8dda263a57b43017)
file(DOWNLOAD ${resource_url_base}/testlm.nnet ${CMAKE_CURRENT_SOURCE_DIR}/rnn/testlm.nnet
        SHOW_PROGRESS EXPECTED_MD5 ccb208512a7148cf00df567fd0da8557)

set(JPP_TEST_RESOURCE_DIR ${CMAKE_CURRENT_SOURCE_DIR} PARENT_SCOPE)